pipeline {
  agent any
  stages {
    stage('S1') {
      parallel {
        stage('S1') {
          steps {
            echo 'toto'
          }
        }
        stage('Firefox') {
          steps {
            build 'job1'
          }
        }
        stage('IE') {
          steps {
            sleep 5
          }
        }
      }
    }
    stage('S2') {
      steps {
        echo 'tii'
      }
    }
  }
}