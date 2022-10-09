pipeline{
    agent any
    stages{
        stage('Build'){
           steps{
            echo 'Build'
            sh 'mvn clean package'
           }
        }
        stage('Test'){
            steps{
                echo 'Test'
                sh mvn 'test'
            }
        }
       stage('Deploy QA'){
            steps{
                echo 'Deploy to QA'
            }
        } 
        stage('Prod'){
            steps{
                echo 'Prod'
            }
        }
    }
    post{
        success{
            echo 'success'
        }
        failure{
            echo 'failed'
        }

    }
}
