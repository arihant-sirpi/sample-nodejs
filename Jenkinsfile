pipeline {
  agent any
    
  stages {

   stage('Pull_git') {
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

   stage('push') {
     steps {
    
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
