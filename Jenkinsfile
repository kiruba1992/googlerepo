pipeline {
  agent any
  stages {
    stage('pre') {
      steps {
        git(url: 'https://github.com/kiruba1992/java.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        sh 'docker --version && docker-compose --version && php --version && composer --version && ls -l ${WORKSPACE}/'
      }
    }
  }
}