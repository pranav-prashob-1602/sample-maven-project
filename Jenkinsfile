pipeline {
  agent any
  stages {
    stage('maven install') {
      steps {
//         echo 'Hello world!'
//         succcess {
          withMaven(maven: 'Maven3') {
            echo 'Hello'
            sh 'mvn clean install'
          }
//         }
      }
    }
  }
}
