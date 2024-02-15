pipeline {
    agent any
    tools {
       tool: 'nodejs'
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