pipeline {
  agent any
  stages {
    stage ("Build") {
      steps {
        echo 'Build automation'
        sh './gradlew build --no-daemon'
        archiveArtifact artifact: 'dist/trainSchedule.zip'
      }
    }
  }
}
