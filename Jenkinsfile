pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage('Docker Build'){
            steps{
               powershell 'Write-Output "Hello, World!"'
            }
        }
         
    }
}