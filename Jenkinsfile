pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        bat './gradlew build'
      }
    }

    stage('Test') {
      steps {
        bat './gradlew clean test'
      }
    }

    stage('Analyze') {
      steps {
        bat './gradlew tasks'
        bat './gradlew sonarqube'
      }
    }

  }
}
