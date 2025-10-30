pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                 git branch: 'main', url: 'https://github.com/Kasulanavya/mobile-cicd-optimization.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Example: sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example: sh './gradlew test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
    post {
        always {
            echo 'Pipeline complete!'
        }
    }
}
