pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t java-docker-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run java-docker-app'
            }
        }
    }
}
