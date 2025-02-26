pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                script {
                    echo 'Cloning repository...'
                    git branch: 'main', url: 'https://github.com/hnp31/Java-CI-CD-Pipeline.git'
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    echo 'Building project...'
                    sh 'mvn clean package'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Running tests...'
                    sh 'mvn test'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying application...'
                }
            }
        }
    }
}
