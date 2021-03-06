pipeline {
    agent any
    def workspace = pwd()
    
    stages {
        stage('Find app') {
            steps {
                echo $workspace
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
