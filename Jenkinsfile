pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sh 'echo "Hello Stage1"'
          }
        }

        stage('Stage1.1') {
          steps {
            sh '''sleep 5
echo "Hello Parallel stage 1.1 "'''
          }
        }

        stage('Stage1.2') {
          steps {
            sh '''sleep 5

echo "Hello Stage 1.2"'''
          }
        }

      }
    }

    stage('Stage2') {
      steps {
        sh 'echo "Hello Stage2"'
      }
    }

    stage('Stage3') {
      parallel {
        stage('Stage3') {
          steps {
            sh 'echo "Hostname is : `hostname`"'
          }
        }

        stage('Satge3.1') {
          steps {
            sh 'echo "Your IP address is : `hostname -I`"'
          }
        }

      }
    }

  }
}