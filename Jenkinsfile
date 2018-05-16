pipeline {
  agent none
  stages {
    stage('docker build') {
      agent {
        dockerfile {
          filename 'Dockerfile'
        }

      }
      steps {
        build 'docker build'
      }
    }
  }
}