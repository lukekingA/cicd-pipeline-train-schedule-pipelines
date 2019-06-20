pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-damon'
        archiveArtifacts artifacts: dist/traneSchedule.zip
      }
    }
  }
}
