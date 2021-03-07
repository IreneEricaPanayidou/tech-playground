pipeline {
    agent any

    stages {
        stage('Find app') {
            steps {
                sh "echo $pwd
                ls -la
                "
            }
        }
        stage('Test') {
            steps {
                sh "
                #!/bin/bash -le
                docker build -t trg-test .
                "
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
