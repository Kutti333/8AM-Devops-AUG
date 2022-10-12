pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sh 'echo "This is stage1"'
          }
        }

        stage('Stage1.1') {
          steps {
            sh '''sleep 5
echo "This is parallel stage1.1"'''
          }
        }

        stage('Stage1.2') {
          steps {
            sh '''sleep 5
echo "this is from stage1.2"'''
          }
        }

      }
    }

    stage('Stage2') {
      steps {
        sh 'echo "This is stage2"'
      }
    }

  }
}