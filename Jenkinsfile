pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation with 99 miles left'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts:'dist/trainSchedule.zip'
      }
    }
  }
}
