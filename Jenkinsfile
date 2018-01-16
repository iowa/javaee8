pipeline {
  agent any
  stages {
    stage('GIT') {
      parallel {
        stage('GIT') {
          steps {
            git(url: 'https://github.com/iowa/javaee8.git', branch: 'master')
          }
        }
        stage('MAVEN') {
          steps {
            sh 'mvn clean package'
          }
        }
      }
    }
  }
}