pipeline {
  agent {
    node {
      label 'jdk9'
    }
    
  }
  stages {
    stage('Say Hellos') {
      steps {
        echo 'Hello World'
        sh 'java -version'
      }
    }
  }
}