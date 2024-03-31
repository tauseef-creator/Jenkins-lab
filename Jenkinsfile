pipeline {

    agent {
        docker {
            image 'node:10.0.0'
            args '-u root'
        }
    }
    environment { 
        CI = 'true'
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