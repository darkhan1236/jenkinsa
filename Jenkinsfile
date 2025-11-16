pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install dependencies') {
            steps {
                bat 'pip install pytest'
            }
        }

        stage('Run tests') {
            steps {
                bat 'pytest -q'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy step (placeholder)"
            }
        }
    }
}
