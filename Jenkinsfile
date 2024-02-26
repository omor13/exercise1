pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh 'rm -rf exercise1'
            }
        }
        stage('build') {
            steps {
                sh 'docker build -t featureimage ./exercise1'
            }
        }
        stage('test') {
            steps {
                sh 'docker images'
            }
        }
    }
}
