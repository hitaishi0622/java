pipeline {
    agent any

    stages {
        stage('git') {
            steps {
                git 'https://github.com/hitaishi0622/java.git'
            }
        }
    }
     stages {
        stage('docker build and run') {
            steps {
                sh '''docker build -f Dockerfile.java -t img1 .
                docker run --name java-container img1'''
            }
        }
    }
}
