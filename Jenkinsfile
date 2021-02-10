pipeline {
  agent any
  stages {
    stage('Test1Stage') {
      steps {
        sh 'docker build -t jayashreelp/python-flask-docker .'
        sh 'docker run --name jaya-container -d -p 8888:8080 jayashreelp/python-flask-docker'
      }
    }

  }
  environment {
    Dev = 'Dev'
  }
}