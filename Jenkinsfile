pipeline {
    agent any
    
    tools {
        // Define Node.js tool with a specific version
        nodejs 'nodejs' // This should match the name configured in Jenkins NodeJS installations
    }
    
    stages {
        stage('Install Dependencies') {
            steps {
                // Install project dependencies using npm
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                // Build the project
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the project
                sh 'npm run deploy'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline succeeded! Congratulations!'
        }
        failure {
            echo 'Pipeline failed! Please check logs for details.'
        }
        always {
            echo 'Pipeline completed.'
        }
    }
}
