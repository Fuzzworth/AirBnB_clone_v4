pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        pwd(tmp: true)
        git(url: 'https://github.com/MODISAR/Thuo_Letlotlo.git', branch: 'master', changelog: true, poll: true)
      }
    }

  }
}