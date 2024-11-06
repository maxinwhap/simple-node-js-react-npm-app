pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'npm install'
                script{
			        powershell '''
				        Write-Output "Hello World!"
				        $date = Get-Date
				        Write-Output "Current Date and Time : $date"
			        '''
                }
                script{
                    powershell '''C:\\Users\\admin01\\Documents\\myscript.ps1'''
                }
            }
        }
    }
}