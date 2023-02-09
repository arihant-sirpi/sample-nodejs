pipeline {
  agent any
    
  stages {
        
     
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
