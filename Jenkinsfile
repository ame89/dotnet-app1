pipeline {
    agent any

    stages {
        stage('shell') {
            steps {
                sh 'echo "Hello World"'
                sh 'echo $PWD'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -al
                '''
            }        
        }
        stage('groovy') {
            steps {
                script {
                    println 'inside script'
                }
            }
        }
    }
}
