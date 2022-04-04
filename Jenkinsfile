pipeline {
  agent any
  stages {
    stage('Prepare') {
      agent any
      steps {
        git(url: 'https://github.com/Stl29/JavaJunitWar.git', branch: 'main')
      }
    }

    stage('build') {
      steps {
        sh 'echo "hello word bis"'
      }
    }

  }
}