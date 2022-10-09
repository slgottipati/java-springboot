pipeline {
    // where or who
    agent any
    
    // collection of stages
    stages{
        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Package'){
            steps{
                sh 'mvn clean package -Dmaven.test.skip=true'
            }
        }
        stage('Deploy war'){
            steps{
                echo 'Deploy'
            }
        }
    }
    post{
        failure{
            echo 'Build Failed'
        }
        success{
            echo 'Build Success'
        }
    }
}