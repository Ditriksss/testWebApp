pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                sh 'dotnet test'
            }
        }
		
		stage('publish') {
            steps {
                sh 'dotnet publish testWebApp/testWebApp.csproj -c Release -o testWebApp/publish/'
            }
        }
    }
}