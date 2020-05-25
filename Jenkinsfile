pipeline {
  agent any
  stages {
    stage('Build, Teste, Validate, Deploy') {
      steps {
        echo 'pull and build'
        sh 'gradle build'
      }
    }

  }
}