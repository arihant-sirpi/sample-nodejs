pipeline {
  agent any
    
  stages {
     
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
