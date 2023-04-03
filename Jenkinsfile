pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'sudo npm install -g http-server'
                sh 'http-server'
            }
        }
        
        stage('Stop') {
            steps {
                sh 'kill $(lsof -t -i:8080)'
            }
        }
    }
}

