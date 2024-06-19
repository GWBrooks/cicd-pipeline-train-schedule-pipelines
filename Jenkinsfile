pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Runnign build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }  
    }
  }
}
