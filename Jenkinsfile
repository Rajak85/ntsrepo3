pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        git(url: 'https://github.com/Rajak85/ntsrepo3.git', branch: 'main', credentialsId: '2c7b884a-097d-4387-8c5e-615e9552a1df')
      }
    }

    stage('Terraform') {
      steps {
        bat 'terraform init'
      }
    }

    stage('Deploy') {
      steps {
        bat 'echo "Blue Ocean Script Executed"'
      }
    }

  }
}