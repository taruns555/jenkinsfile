pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            git(url: 'https://github.com/taruns555/jenkinsfile.git', branch: 'master', poll: true)
          }
        }
        stage('') {
          steps {
            git(url: 'https://github.com/taruns555/jenkinsfile.git', branch: 'slave', poll: true)
          }
        }
      }
    }
  }
}