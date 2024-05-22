pipeline {

     agent { 
        node {
            label 'alex-jenkins-alpine-new'
            }
      }
  stages {
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    stage('hello') {
      steps {
        sh 'python3 hello.py'
      }
    }
  }
}
