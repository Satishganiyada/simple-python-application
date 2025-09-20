pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git branch: 'main', url: 'https://github.com/Satishganiyada/simple-python-application'
                echo 'Hello World'
                sh 'sudo docker build -t python:v1 .'
                sh 'sudo docker compose up -d'

            }
        }
    }
}



