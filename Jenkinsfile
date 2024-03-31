pipeline {

    agent any
    stage('Pull Docker Image') {
            steps {
                script {
                    // Pull the Node.js Docker image
                    docker.image('node:latest').pull()
                }
            }
        }
    stages {
         stage('build') {
          steps {
              bat 'npm install'
            }
          }
        
        stage('Docker Comopse Up') {
            steps {
               
                    bat "docker compose up"
                
            }
        }
    }
}