pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Run') {
            steps {
                sh 'docker run --rm -d -p 8081:80 nginx:alpine'
            }
        }
    }

}
