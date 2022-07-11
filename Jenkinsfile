pipeline {
  agent any
  stages {
    stage('maven install') {
      steps {
        withMaven(maven: 'Maven3') {
            sh 'mvn clean install'
        }
      }
    }
    stage('publish') {
      steps {
        sh './mvnw package'
      }
      post {
        success {
          archiveArtifacts 'target/*.jar'
        }
      }
    }
  }

  
}
