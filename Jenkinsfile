pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ main/output.cpp -o output'
      }
    }
    stage('Test') {
      steps {
        sh './output'
      }
    }
    stage('deploy') {
      steps {
        echo 'deployed!'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
