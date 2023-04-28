pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(url: 'https://github.com/dkalarus/jenkins', branch: 'dev')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('error') {
      steps {
        sh '''docker --version
docker pull alexwhen/docker-2048
docker run -d -p 5000:80 alexwhen/docker-2048'''
      }
    }

  }
}