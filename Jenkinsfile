pipeline {
  agent any
  stages {
    stage('Build, Teste, Validate, Deploy') {
      steps {
        sh './gradle build'
        echo 'pull and build'
      }
    }

  }
}