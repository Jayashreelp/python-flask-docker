pipeline {
  agent any
  stages {
    stage('Test1Stage') {
      steps {
        sh 'docker build -t python-flask-docker .'
      }
    }

  }
  environment {
    Dev = 'Dev'
  }
}