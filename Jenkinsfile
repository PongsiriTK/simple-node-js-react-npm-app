pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
                powershell '''
                    Write-Output "Hello World"
                    $date = Get-Date
                    Write-Output "Current Date and time : $date"
                '''
            }
        }
    }

}