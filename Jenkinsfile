pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
                echo 'from powershell command'
                powershell '''
                    Write-Output "Hello World"
                    $date = Get-Date
                    Write-Output "Current Date and time : $date"
                '''
                echo 'from file'
                powershell "C:\\test-script\\myscript.ps1"
            }
        }
    }

}