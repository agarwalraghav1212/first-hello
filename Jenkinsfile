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
                sh 'pm2 start index.js'
            }
        }
        stage('show'){
            steps{
                sh 'pm2 list'
            }
        }    
    }
}
