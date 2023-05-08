pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                dotnetBuild "${workspace}/src/com.github.ame89.app1.csproj"
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
