pipeline {
  agent any 
  stages {
    stage ('Build') {
      steps {
        echo "Running Automation build"
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        }
      }
  }
 }
