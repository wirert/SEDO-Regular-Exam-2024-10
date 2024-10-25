pipeline {
    agent any 
    stages {
        stage('Restore dependancies') { 
            steps {
                bat 'dotnet restore' 
            }
        }
        stage('.Net Build') { 
            steps {
                bat 'dotnet build' 
            }
        }
        stage('Run tests') { 
            steps {
                bat 'dotnet test --no-build --verbosity normal' 
            }
        }
    }
}
