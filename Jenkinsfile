pipeline {
  agent {
    label 'docker' 
  }
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

    stage('Build') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile .'
      }
    }

  }
}
