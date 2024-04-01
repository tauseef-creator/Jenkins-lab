pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/tauseef-creator/Jenkins-lab'
            }
        }

        stage('Dependency Installation') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Containerize and Deploy') {
            steps {
                sh "docker compose up"
            }
        }

        stage('Kill') {
            steps {
                sh "docker compose down"
            }
        }
    }
}
