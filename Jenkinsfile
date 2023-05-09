pipeline {
    agent any

    stages {
        stage('shell') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
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
