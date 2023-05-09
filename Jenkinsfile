pipeline {
    agent any

    stages {
        stage('Pre') {
            steps {
                echo 'Pre..'
                sh {
                    "ls -al"
                }
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                script {
                    dotnetBuild "${workspace}/src/com.github.ame89.app1.csproj"                   
                }
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
