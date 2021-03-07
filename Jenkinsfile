pipeline {
    agent any

    stages {
        stage('Find app') {
            steps {
                sh """
                #!/bin/bash -le
                echo $pwd
                ls -la
                """
            }
        }
        stage('Test') {
            steps {
                sh """
                #!/bin/bash -le
                docker build -t trg-test .
                """
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
