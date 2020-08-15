pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo " This is $BUILD_NUMBER of $demo "'
      }
    }

    stage('Test') {
      steps {
        echo 'Hello Test'
      }
    }

  }
  environment {
    demo = '1'
  }
}