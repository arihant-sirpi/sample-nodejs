pipeline {
  agent any
    
  stages {
        
    stage('Git') {
      steps {
        git 'git@github.com:arihant-sirpi/sample-nodejs.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh 'node app.js'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
