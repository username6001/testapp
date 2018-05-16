pipeline {
  agent any
  stages {
    stage('build docker image') {
      steps {
        sh 'docker build -t gcr.io/alan-stage/testapp .'
      }
    }
  }
}