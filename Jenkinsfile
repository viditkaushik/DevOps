pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t prizm-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat 'docker stop prizm-container || exit 0'
                bat 'docker rm prizm-container || exit 0'
                bat 'docker run -d -p 5000:5000 --name prizm-container prizm-app'
            }
        }
    }
}