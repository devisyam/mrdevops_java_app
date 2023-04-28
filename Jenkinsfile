@Library('variable') _

pipeline{

    agent any
    stages {
        stage('git checkout') {
            steps {
            gitCheckout(
                 branch: "main",
                 url: "https://github.com/devisyam/mrdevops_java_app.git"
            )
            }
        }
        stage('Unit Test Maven'){
            steps{
                script{
                    
                    mvnTest()
                }
            }
        }
        stage('integration test maven') {
            steps {
                script{
                    
                    mvnIntegrationTest()
                }
            }
        }
    }
}

   
