pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      
      sh 'g++ -o deven simple.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './deven'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
