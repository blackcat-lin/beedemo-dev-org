pipeline {
  agent {
    node {
      label 'jdk8'
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