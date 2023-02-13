pipeline {
  agent any
    
  stages {

    stage('pull') {
      steps {   
        git branch: 'main', credentialsId: 'at', url: 'git@github.com:arihant-sirpi/sample-nodejs.git'
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
