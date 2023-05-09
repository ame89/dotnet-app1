pipeline {
    agent any

    stages {
        stage('shell') {
            steps {
                sh "echo $SHELL"
                sh "ls -al"
            }
        }
        stage('groovy') {
            steps {
                script {
                    println 'inside script'
                }
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                script {
                    //dotnetBuild "${workspace}/src/com.github.ame89.app1.csproj"
                    println 'groovy'                   
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
