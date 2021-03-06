def PATH
pipeline {
    agent any
    
    stages {
        stage('Find app') {
            steps {
                sh "PATH = $(pwd)"
                echo $PATH
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
