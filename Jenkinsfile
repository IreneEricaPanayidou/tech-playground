def PATH
pipeline {
    agent any
    
    stages {
        stage('Find app') {
            steps {
               echo 'Something'
            }
        }
        stage('Containerizing application') {
            steps {
                sh '''  docker build -t trg-assignment .
                   '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
