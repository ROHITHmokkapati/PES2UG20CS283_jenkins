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
        sh '/var/jenkins_home/workspace/PES2UG20CS283/ran'
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
