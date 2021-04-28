pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo "Running Build automation"
        sh "./gradlew build --no-dameon"
        archiveArtifacts artifacts: "dist/trainSchedule.zip"
      }
    }
  }
}
