pipeline {
    agent any
    parameters {
      string defaultValue: 'https://github.com/omor13/exercise1.git', name: 'url'
    }
    stages {
        stage('clone') {
            steps {
                sh 'rm -rf exercise1'
                sh 'git clone ${url}'
            }
        }
        stage('build') {
            steps {
                sh 'docker build -t prodImage ./exercise1'
            }
        }
        stage('test') {
            steps {
                sh 'docker images'
            }
        }
    }
}
