node {
    stage('Checkout') {
        git 'https://github.com/hnp31/Java-CI-CD-Pipeline.git'
    }
    stage('Build') {
        sh 'mvn clean package'
    }
    stage('Test') {
        sh 'mvn test'
    }
    stage('Deploy') {
        echo 'Deploying application...'
    }
}
