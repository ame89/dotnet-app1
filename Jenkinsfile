pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                dotnet build com.github.ame89.app1.csproj
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
