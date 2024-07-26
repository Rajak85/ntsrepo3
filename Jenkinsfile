pipeline {
    agent any

    stages {
        stage('1') {
            steps {
                git branch: 'main', credentialsId: '2c7b884a-097d-4387-8c5e-615e9552a1df', url: 'https://github.com/Rajak85/ntsrepo3.git'
            }
        }
      stage('2') {
            steps {
                bat 'terraform init'
            }
        }
      stage('3') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
