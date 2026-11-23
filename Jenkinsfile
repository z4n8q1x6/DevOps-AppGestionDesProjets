pipeline {
    agent any

    options {
        skipDefaultCheckout()
    }

    stages {
        stage('Git Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -f backend/pom.xml clean compile'
            }
        }
    }
}
