pipeline {
  agent {
    docker {
      image 'library/busybox'
      args '-v /Documents/busybox'
    }
    
  }
  stages {
    stage('BusyBox shell') {
      steps {
        sh 'echo \'Aloha mate\''
      }
    }
    stage('Arch') {
      steps {
        archiveArtifacts '*'
      }
    }
  }
}