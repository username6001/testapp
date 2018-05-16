pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Build image') {
      app = docker.build("[id-of-your-project-as-in-google-url]/[name-of-the-artifact]")
    }
    stage('Push image') {
      docker.withRegistry('https://gcr.io', 'gcr:[credentials-id]') {
        app.push("${env.BUILD_NUMBER}")
        app.push("latest")
      }
    }
  }
}