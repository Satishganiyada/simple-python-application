pipeline {
    agent any

    stages {
        stage('build and deploy') {
            steps {
                git branch: 'main', url: 'https://github.com/Satishganiyada/simple-python-application'
                sh 'sudo docker build -t python:v1 .'
                sh 'sudo docker compose up -d'
            }
        }
    }
}