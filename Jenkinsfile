pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
              
                sh 'make' 
                archiveArtifacts artifacts: '**/app/*.php', fingerprint: true 
           
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
