pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                bat "dotnet build"
            }
        }
        stage("Test"){
            steps{
                bat "dotnet test"
            }
        }
    }
    post{
        always{
            echo "always"
        }
        success{
            echo "pipeline executed successfully"
        }
        failure{
            echo "pipeline execution failed"
        }
    }
}