pipeline {
  agent any
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/agarwalraghav1212/first-hello.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'npm start index.js'
      }
    }
  }
}
