pipeline {
  agent any
  stages {
    stage('Test1Stage') {
      steps {
        sh 'docker build -t jayashreelp/python-flask-docker .'
        sh 'docker run -p 8888:8080 python-flask-docker'
      }
    }

  }
  environment {
    Dev = 'Dev'
  }
}