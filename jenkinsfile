pipeline{
    agent any
    tools{
        maven 'maven3.9.6'
    }
    stages{
        stage('1.GitHubCodeCheckout'){
            steps{
                git "https://github.com/fvder/easybuggy-vulnerable-application.git"
            }
        }
        stage('2.Build'){
            steps{
                sh "mvn clean package"
            }
        }
 /*       stage('3.SonarQubeSAST/SCQA'){
            steps{
                sh "mvn sonar:sonar"
            }
        } */
    }
}
