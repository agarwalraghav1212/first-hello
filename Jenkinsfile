pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'npm i'
            }
        }
        stage('Test') {
            steps {
                sh 'npm start index.js'
            }
        }
        stage('show'){
            steps{
                sh 'npm list'
            }
        }    
    }
}
