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
                //   git branch: 'main', url: 'https://github.com/Parsu1508/devops.git'

                
            }
        }
    }
}