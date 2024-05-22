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
               stage('Build') {
            steps {
                echo "Building.."
                sh '''
                pip install -r requirements.txt
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                python3 hello.py
                python3 hello.py --name='Alexandre Meli'
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                
                 script{
                     echo "doing other stuff"
                     ls
                     pwd
                }
            
            }
        }
    stage('hello') {
      steps {
        sh 'python3 hello.py'
      }
    }
  }
}
