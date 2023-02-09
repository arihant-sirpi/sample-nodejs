pipeline {
  agent any
    
  tools {'nodejs'}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'git@github.com:arihant-sirpi/sample-nodejs.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
