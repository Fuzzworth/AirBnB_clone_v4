pipeline {
  agent any
  stages {
    stage('Git install') {
      steps {
        sh 'apt install git'
      }
    }

    stage('Checkout') {
      steps {
        git(url: 'https://github.com/Fuzzworth/AirBnB_clone_v4.git', branch: 'master', changelog: true, poll: true)
      }
    }

    stage('List') {
      steps {
        sh 'ls -la'
      }
    }

  }
}