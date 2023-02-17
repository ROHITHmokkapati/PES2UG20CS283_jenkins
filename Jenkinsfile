pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ rand.cpp -o rand'
        echo 'built'
      }
    }
    
    stage('Test') {
      steps {
        sh './rand'
        echo 'test!!'
      }
    }
    
    stage('Deploy') {
      steps {
        echo 'Deployed!'
      }
    }
  }
  
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
