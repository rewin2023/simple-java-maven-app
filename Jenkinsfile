pipeline {
    agent any
    stages {
        stage('Checkout22') {
            steps {
                git url: 'git@github.com:rewin2023/simple-java-maven-app.git', credentialsId: 'github-key', branch: 'master'
            }
        }
        stage('Show files') {
            steps {
                sh 'ls -al'
            }
        }
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}

