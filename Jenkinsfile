pipeline {
  agents any
  stages {
    stage ('build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts atifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
