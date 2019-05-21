pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build automation'
        sh './gradlew build --no-daemon'
        archiveArtifact artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
