pipeline {
    agent any
    tools {
      nodejs 'node-16'
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