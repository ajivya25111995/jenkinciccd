pipeline {
    agent none

    stages {

        stage('Checkout') {
            agent any
            steps {
                checkout scm
            }
        }

        stage('Test') {
            agent any
            steps {
                echo 'GitHub checkout successful'
                echo 'Declarative Pipeline is working'
            }
        }
    }
}