pipeline {
  agent any
  stages {
    stage('Test1Stage') {
      steps {
        sh 'docker build .'
      }
    }

  }
  environment {
    Dev = 'Dev'
  }
}