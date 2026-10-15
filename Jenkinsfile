
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Starting Jenkins CI/CD pipeline'
                checkout scm
            }
        }

        stage('Check Project') {
            steps {
                sh 'pwd'
                sh 'ls -la'
                echo 'Project files checked successfully'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage completed'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the console output.'
        }
    }
}
