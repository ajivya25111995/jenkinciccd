pipeline {
    agent any

    stages {

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