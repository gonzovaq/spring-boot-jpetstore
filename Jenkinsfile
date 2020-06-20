pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sh './gradlew build'
      }
    }

    stage('Test') {
      steps {
        sh './gradlew clean test'
      }
    }

    stage('Analyze') {
      steps {
        sh './gradlew sonarqube'
      }
    }

  }
}