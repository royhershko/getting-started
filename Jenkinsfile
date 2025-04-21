pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/royhershko/getting-started.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'chmod +x build.sh'
                    sh './build.sh'
                }
            }
        }
    }
}
