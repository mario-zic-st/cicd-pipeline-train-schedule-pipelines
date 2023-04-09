pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        println 'Starting build ..'
        sh './gradlew build --no-daemon'
        println 'List artifacts ..'
        sh 'ls -la ./dist/*'
        // archive
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
