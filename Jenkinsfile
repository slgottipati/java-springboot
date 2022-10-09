pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo 'Build'               
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Push to Artifactory') {
            steps {
                echo 'Push to Artifactory'
            }
        }
        stage('Deploy to QA') {
            steps {
                echo 'Deploy to QA'
            }
        }

        stage('Deploy to Prod') {
            steps {
                echo 'Deploy to Prod'
            }
        }
    }
    post {
      failure {
        echo 'Failed'
      }
      success {
        echo 'Success'
      }
      aborted {
        echo 'aborted'
      }
    }
}