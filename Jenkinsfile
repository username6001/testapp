pipeline {
  agent any
  stages {
    stage('build image') {
      steps {
        sh 'docker build -t gcr.io/alan-stage/testapp .'
      }
    }
    stage('push to gcr') {
      steps {
        sh 'docker push gcr.io/alan-stage/testapp'
      }
    }
  }
}