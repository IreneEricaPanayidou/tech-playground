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
                sh ''' FROM python:3
    
                        ADD hello_world.py /

                        RUN pip install flask

                        CMD [ "python", "./hello_world.py" ]
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
