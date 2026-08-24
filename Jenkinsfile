pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out GitHub repository'
            }
        }

        stage('Build') {
            steps {
                echo 'Building HTML project'
            }
        }

        stage('Test') {
            steps {
                bat 'if exist index.html (echo index.html found) else (exit /b 1)'
            }
        }

        stage('Success') {
            steps {
                echo 'Pipeline completed successfully!'
            }
        }
    }
}
