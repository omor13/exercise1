pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                sh 'echo "Branch Checkout"'
            }
        }
        stage('build') {
            steps {
                sh 'docker build -t featureimage .'
            }
        }
        stage('test') {
            steps {
                sh 'docker images'
            }
        }
    }
}
