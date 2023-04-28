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
    }
}

   
