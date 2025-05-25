pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'git@github.com:rewin2023/simple-java-maven-app.git', credentialsId: 'github-key', branch: 'master'
            }
        }
        stage('Show files') {
            steps {
                sh 'ls -al'
            }
        }
    }
}

