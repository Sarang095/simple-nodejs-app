pipeline {
    agent any

    tools {
        nodejs 'NODEJS25'    
    }

    stages {
        stage('Checkout code'){
            steps{
                checkout scm
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }


        stage('Start application') {
            steps {
                sh 'npm start &'
            }
        }
    }
}
