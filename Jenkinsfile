pipeline{
    agent any
    stages{
        stage('Build')
        steps{
            echo 'Build'
        }
        stage('Test'){
            steps{
                echo 'Test'
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
