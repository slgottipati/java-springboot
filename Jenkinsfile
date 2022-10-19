pipeline{
    agent any
    stages{
        stage('Test'){
            steps{
            echo 'Test'
            sh 'mvn test'
            }
        }   
        stage('Build'){
            steps{
                echo 'Build'
                sh 'mvn clean package'
            }
        }    
            stage('Push to Artifactory'){
                steps{
                    echo 'Push to Artifactory'
                }
            }
            stage('Deploy to Dev'){
                steps{
                    echo 'Deploy to Dev'
                }
            }
            stage('Deploy to QA'){
                steps{
                    echo 'Deploy to QA'
                }
            }
            stage('Deploy to UAT'){
                steps{
                    echo 'Deploy to UAT'
                }
            }
            stage('Deploy to staging'){
                steps{
                    echo 'Deploy to staging'
                }
            }
            stage('Deploy To Prod'){
                steps{
                    echo 'Deploy to Prod'
                }

            }
    }
            post{
                failure{
                    echo 'Failed'
                }
                success{
                    echo 'Success'
                }
            }
        
        }
    
