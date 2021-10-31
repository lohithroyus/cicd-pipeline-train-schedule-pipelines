pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo "Running Build automation1"
        sh "./gradlew build --no-daemon"
        archiveArtifacts artifacts: "dist/trainSchedule.zip"
      }
    }
  }
}
