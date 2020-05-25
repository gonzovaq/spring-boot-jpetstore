pipeline {
  agent any
  stages {
    stage('Build, Teste, Validate, Deploy') {
      steps {
        sh './gradlew build'
        echo 'pull and build'
      }
    }

  }
}