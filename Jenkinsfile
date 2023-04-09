pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        println 'Starting build ..'
        sh './gradlew build'
        println 'List artifacts ..'
        sh 'ls -la ./dist/*'
      }
    }
  }
}
