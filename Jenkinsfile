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
      agent any
      steps {
        sh 'mvn clean install'
      }
    }

    stage('test') {
      agent any
      steps {
        sh 'mvn clean test'
      }
    }

  }
}