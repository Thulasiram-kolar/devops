pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "stage1"'
          }
        }

        stage('parallel1') {
          steps {
            sh 'echo "hello parallel_1"'
          }
        }

        stage('parallel2') {
          steps {
            sh 'echo "hello parallel_2"'
          }
        }

      }
    }

    stage('stage2') {
      steps {
        sh 'echo "hello stage2"'
      }
    }

    stage('stage3') {
      steps {
        sh 'echo "hello stage 3"'
      }
    }

  }
}