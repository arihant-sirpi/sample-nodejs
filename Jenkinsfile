pipeline {
  agent any
    
  stages {

    stage('pull') {
      steps {   
        git 'https://github.com/arihant-sirpi/sample-nodejs.git'
      }
     }
    stage('Build') {
      steps {
        sh 'npm install'
         sh 'nohup npm start'
      }
     }    
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
