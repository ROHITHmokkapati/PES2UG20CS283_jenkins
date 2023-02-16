pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh 'g++ hello.cpp -o hello'
            }
        }
        stage('test') {
            steps {
                sh './hello'
            }
        }
        stage('deploy') {
            steps {
            }
        }
    }
    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
