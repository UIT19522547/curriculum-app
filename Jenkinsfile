pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/UIT19522547/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-End Unit Tests / Shell script') {
          steps {
            sh 'cd curriculum-front && npm i'
          }
        }

      }
    }

  }
}