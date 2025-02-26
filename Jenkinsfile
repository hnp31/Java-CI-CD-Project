pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    echo '🔄 Cloning repository...'
                    git branch: 'main', url: 'https://github.com/hnp31/Java-CI-CD-Pipeline.git'
                }
            }
        }
        stage('Verify Workspace') {
            steps {
                script {
                    echo '📂 Checking workspace contents...'
                    sh 'ls -la'
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    echo '⚙️ Building project...'
                    sh 'mvn clean package'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo '🧪 Running tests...'
                    sh 'mvn test'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    echo '🚀 Deploying application...'
                }
            }
        }
    }
}
