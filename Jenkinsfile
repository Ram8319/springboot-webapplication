pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/Ram8319/springboot-webapplication.git', branch: 'main', credentialsId: 'git-token')
      }
    }

    stage('docker-login') {
      steps {
        sh 'docker login'
      }
    }

  }
}