pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        powershell './gradlew build'
      }
    }

    stage('Test') {
      steps {
        powershell './gradlew clean test'
      }
    }

    stage('Analyze') {
      steps {
        powershell './gradlew tasks'
        powershell './gradlew sonarqube'
      }
    }

  }
}
