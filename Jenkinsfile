pipeline {
  environment {
        registry = 'jayashreelp'
        registryCredential = 'dockerid'
        dockerImage = ''
      }
  agent any
  stages {
    stage('Building our image') { 
      steps {
        sh 'dockerImage = docker.build registry + ":$BUILD_NUMBER"'
      }
    }

    stage('Deploy our image') {
      steps {
        sh '''docker.withRegistry( \'\', registryCredential ) {
dockerImage.push()'''
        }
      }

    }
    }
  }
