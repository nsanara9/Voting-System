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
    
    
    stage('Start test app'){
        steps{
            docker-compose up -d
            ./scripts/test_container.ps1
        }
        
        post{
            success{
                echo "App started successfully :)"
            }
            failiure{
                echo "App failed to start :("
            }
        }
    }
    
    stage('Run Tests'){
        steps{
          powershell 'Write-Output "Hello, World!"'  
        }
    }
    stage('stop test app'){
        steps{
           powershell 'Write-Output "Hello, World!"' 
        }

}
}   
}
        