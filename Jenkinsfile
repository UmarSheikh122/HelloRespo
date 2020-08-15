pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo " This is $BUILD_NUMBER of $demo "'
      }
    }

  }
  environment {
    demo = '1'
  }
}