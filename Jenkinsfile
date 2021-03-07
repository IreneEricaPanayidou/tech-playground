pipeline {
    agent any

    stages {
        stage('Initialize'){
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
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
