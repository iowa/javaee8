pipeline {
  agent any
  stages {
    stage('Download') {
      steps {
        git(url: 'https://github.com/iowa/javaee8.git', branch: 'master', changelog: true, poll: true)
      }
    }
  }
}