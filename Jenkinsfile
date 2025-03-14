pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o output hello.cpp'
            }
        }
        stage('Test') {
            steps {
                sh './output'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment Stage: Simulating Deployment'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed'
        }
    }
}
