pipeline {
  agent any
  stages {
    stage('maven install') {
      steps {
        withMaven(maven: 'Maven3') {
            echo 'Hello'
            sh 'mvn clean install'
        }
      }
    }
  }
}
