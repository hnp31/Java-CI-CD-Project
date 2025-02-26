pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/hnp31/Java-CI-CD-Pipeline.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
