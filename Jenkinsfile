pipeline {
    agent any
    // agent {
    //     docker {
    //         image 'node:10.0.0'
    //         args '-u root'
    //     }
    // }
    // environment { 
    //     CI = 'true'
    // }
    stages {
         stage('build') {
          steps {
              sh 'npm install'
            }
          }
        
        // stage('Docker Comopse Up') {
        //     steps {
               
        //             sh "docker compose up"
                
        //     }
        // }
    }
}