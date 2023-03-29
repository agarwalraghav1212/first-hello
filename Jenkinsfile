pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'npm i'
            }
        }
         stage('Publish') {
         steps {
            rtNpmPublisher (
               serverId: 'artifactory',
               repo: 'npm_demo',
               packageJson: 'package.json',
               targetRepo: 'npm_remote_demo',
               publishArtifacts: true
            )
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
