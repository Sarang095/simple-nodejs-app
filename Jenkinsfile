pipeline {
    agent any

    tools {
        nodejs 'NODEJS25'    
    }

    stages {
        stage('Checkout code'){
            steps{
                git branch: 'master', url: 'https://github.com/rat9615/simple-nodejs-app.git'
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
