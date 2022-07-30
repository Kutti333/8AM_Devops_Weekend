pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        sh 'echo "Hello Stage1"'
      }
    }

    stage('Stage2') {
      steps {
        sh 'echo "Hello Stage2"'
      }
    }

    stage('Stage3') {
      steps {
        sh 'echo "Hostname is : `hostname`"'
      }
    }

  }
}