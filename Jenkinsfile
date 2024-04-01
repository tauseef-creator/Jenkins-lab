pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Assuming you've set up your GitHub repository correctly in Jenkins
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
                sh 'npm install' // Assuming 'npm run build' is the command to build your app
            }
        }

        stage('Test') {
            steps {
                sh 'npm test' // Assuming 'npm test' is the command to run your tests
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
