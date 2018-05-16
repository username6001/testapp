pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
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