pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS334 PES2UG20CS334.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS334'
    }
  }

  stage('Deploy') {
    steps{
      echo 'Deployment successful'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
