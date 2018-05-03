pipeline {
  agent {
    node {
      label 'jdk8'
    }
    
  }
  stages {
    stage('Say Hellos') {
      environment {
        MY_NAME = 'foo'
      }
      steps {
        echo 'Hello World'
        sh 'java -version'
      }
    }
  }
}