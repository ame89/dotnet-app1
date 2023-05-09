pipeline {
    agent any

    stages {
        stage('shell') {
            steps {
                sh 'echo $PWD'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -al
                '''
                sh 'echo ${workspace}'
            }        
        }
        stage('groovy') {
            steps {
                script {
                    println 'inside script'
                }
            }
        }
        stage('dotnet') {
            steps {
                sh 'dotnet src/com.github.ame89.app1.csproj'
            }
        }
    }
}
