pipeline {

     agent { 
        node {
            label 'custom-jenkins-agent-phyton'
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
