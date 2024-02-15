pipeline {
    agent any
    tools {
        'node 16', type: 'nodejs'
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