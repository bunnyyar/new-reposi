pipeline {
    agent any
    tools {
     'nodejs'
    } 
    
    stages{
        stage('build') {
            steps{
                sh 'npm install'
                sh 'npm run start'
            }
        }
    }
}