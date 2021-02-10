pipeline {
  agent any
  stages {
    stage('Building our image') {
      environment {
        registry = 'jayashreelp'
        registryCredential = 'dockerid'
        dockerImage = ''
      }
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
    environment {
      registry = 'jayashreelp'
      registrycredentialdockerim = 'dockerid'
    }
  }