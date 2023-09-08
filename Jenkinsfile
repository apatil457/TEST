pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                // Check out your code from Git
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Build your project (e.g., compile code)
                sh './test.sh'
            }
        }

        stage('Test') {
            steps {
                // Run tests (if applicable)
                sh './test.sh'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy your application
                sh './test.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}

