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
            sh 'for i in {1..5}; do echo "hello $i time" && sleep 1; done'
          }
        }

      }
    }

    stage('stage2') {
      steps {
        sh 'echo "hello stage2"'
      }
    }

    stage('stage 3') {
      steps {
        echo 'stage3 added'
      }
    }

    stage('stage4') {
      steps {
        sh 'echo "added stage 4"'
      }
    }

  }
}