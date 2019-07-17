pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/balajireddy8898/simple-java-maven-app.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        powershell ' clean install'
        sh 'mvn clean install'
      }
    }
  }
}