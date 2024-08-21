pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                git branch: 'main', url: 'https://github.com/RafaelMMorais/Teste-API-EBAC.git'
                bat 'npm install'
            }
        }
        stage('Teste') {
            steps {
               bat '''set NO_COLOR=1
               npm start
                npm test'''
            }
        }
    }
}