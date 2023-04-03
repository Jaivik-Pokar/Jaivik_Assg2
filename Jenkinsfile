pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install -g http-server'
                sh 'http-server'
            }
        }
    }
}

