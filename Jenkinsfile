pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "checkout scm"
            }
        }
        stage('Install dependencies') {
            steps {
                echo 'Install dependencies from requirements.txt'
            }
        }
        stage('Run app.py') {
            steps {
                sh 'python3 app.py'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'python3 -m unittest discover'
            }
        }
        stage('Deploy  Code') {
            steps {
                echo 'deploy to ECR from feature branch'
            }
        }
    }
}

   