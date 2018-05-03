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
    stage('Get Kernel') {
      steps {
        script {
          try {
            KERNEL_VERSION = sh (script: "uname -r", returnStdout: true)
          } catch(err) {
            echo "CAUGHT ERROR: ${err}"
            throw err
          }
        }
        
      }
    }
    stage('Say Kernel') {
      steps {
        echo "${KERNEL_VERSION}"
      }
    }
  }
}