pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                echo '🔄 Cloning repository...'
                git branch: 'main', url: 'https://github.com/hnp31/Java-CI-CD-Pipeline.git'
            }
        }
        stage('Build') {
            steps {
                echo '⚙️ Running Maven Build...'
                bat 'cd ABC-Technologies && mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo '✅ Running Tests...'
                bat 'cd ABC-Technologies && mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo '🚀 Deploying Application...'
            }
        }
    }
}
