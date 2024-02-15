pipeline {
    agent any
    tools {
       tool: 'node 16', type: 'nodejs'
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