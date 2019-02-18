pipeline {
  agent any
  stages {
    stage('Commit') {
      steps {
        git(url: 'https://github.com/srini289/TFS.git', branch: 'master', changelog: true, credentialsId: 'srini289', poll: true)
      }
    }
    stage('') {
      steps {
        stash(name: 'sample', includes: '*.txt')
      }
    }
  }
}