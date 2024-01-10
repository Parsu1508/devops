@Library('jenkins-shared-lib') _

pipeline{

    agent any

    stages{
        
        stage("git chckout"){
            steps{ 
                gitCheckout(
                   branch: "main",
                   url: "https://github.com/Parsu1508/devops.git"
                )
            }
        }

         stage("Unit Test mvanen"){
            steps{ 
               script{
                mvntest()
               }
            }
        }

        stage("Integartion Test mvanen"){
            steps{ 
               script{
                mvnIntegartion()
               }
            }
        }

        stage("Static Code Analysis"){
            steps{ 
               script{
                staticCodeAnalysis()
               }
            }
        }
    }
}