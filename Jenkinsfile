pipeline {
    agent any
    
    stages {
        stage('Find app') {
            steps {
                sh 'pwd'
                sh 'ls -la'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
