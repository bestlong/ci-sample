pipeline {
  agent {
    docker {
      image 'node:8.1.0'
      args '-u root'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm i -g yarn'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}
