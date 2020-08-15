pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        sh 'echo " This is $BUILD_NUMBER and demo $demo "'
      }
    }

  }
  environment {
    demo = '1'
  }
}