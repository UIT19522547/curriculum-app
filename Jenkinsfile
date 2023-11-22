pipeline {
  agent any
  stages {
    stage('Checkout code / Git') {
      steps {
        git(url: 'https://github.com/UIT19522547/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

  }
}