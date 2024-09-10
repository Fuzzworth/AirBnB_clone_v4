pipeline {
  agent {
    docker {
      image 'jenkins/jnlp-agent-python3'
    }

  }
  stages {
    stage('Git install') {
      steps {
        sh 'apt-get update --allow-unauthenticated   && apt-get install -y git && rm -rf /var/lib/apt/lists/*'
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