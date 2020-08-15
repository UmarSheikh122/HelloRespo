pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        sh 'echo "THis is build number $BUILD_NUMBER and Demo $demo"'
      }
    }

  }
  environment {
    demo = '1'
  }
}