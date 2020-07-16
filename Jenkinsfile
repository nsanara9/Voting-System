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
           powershell 'Write-Output "Hello, World!"' 
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
        