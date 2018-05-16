pipeline {
  agent none
  stages {
    stage('Build image') {
      app = docker.build("gcr.io/alan-stage/testapp")
    }
    // stage('Push image') {
    //   docker.withRegistry('https://gcr.io', 'gcr:[credentials-id]') {
    //     app.push("${env.BUILD_NUMBER}")
    //     app.push("latest")
    //   }
    // }
  }
}