pipeline {
  agent any
  stages {
    stage('Test1Stage') {
      steps {
        sh 'docker build . -t python-flask-docker-app'
        sh 'docker run --name jaya-container1 -d -p 8888:8080 python-flask-docker-app'
      }
    }

  }
  environment {
    Dev = 'Dev'
  }
}