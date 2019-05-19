pipeline {
  agent any 
  stages ('Build') {
    steps {
      echo 'Running build automation'
      sh './gradlew build --no-daemon'
      archibeArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
