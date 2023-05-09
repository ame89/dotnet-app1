pipeline {
    agent any
    
    environment {
        DOTNET_CLI_TELEMETRY_OPTOUT=1
    }

    stages {
        stage('shell') {
            steps {
                sh 'echo $PWD'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -al
                '''
                sh 'echo ${workspace}'
                sh 'ls -al /var/jenkins_home/tools'
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
                sh '/var/jenkins_home/tools/io.jenkins.plugins.dotnet.DotNetSDK/net7/dotnet build src/com.github.ame89.app1.csproj'
            }
        }
    }
}
