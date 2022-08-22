pipeline {
  agent {
    node {
      label 'Slave'
    }

  }
  stages {
    stage('echo') {
      steps {
        sh 'echo " Hello Blue Ocean" > echo.txt'
        archiveArtifacts(artifacts: 'echo.txt', fingerprint: true)
      }
    }

  }
}