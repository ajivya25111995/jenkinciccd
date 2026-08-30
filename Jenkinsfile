pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Test') {
            steps {
                echo 'GitHub checkout successful'
                echo 'Declarative Pipeline is working'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    rm -rf /var/www/myapp/*
                    cp -r ./* /var/www/myapp/
                '''
            }
        }
    }
}