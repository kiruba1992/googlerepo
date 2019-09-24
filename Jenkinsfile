pipeline {
  agent any
  stages {
    stage('pre') {
      steps {
        git(url: 'https://github.com/kiruba1992/googlerepo.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        sh 'docker --version && docker images'
      }
    }
  }
}