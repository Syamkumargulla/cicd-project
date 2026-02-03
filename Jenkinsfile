pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                echo 'Code already available'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t cicd-demo .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm cicd-demo'
            }
        }
    }
}
