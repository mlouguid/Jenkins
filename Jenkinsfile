pipeline {
  agent none
  stages {
    stage('message') {
      parallel {
        stage('message') {
          steps {
            echo 'hello all'
          }
        }

        stage('Build') {
          steps {
            sh 'build test docker'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'docker '
      }
    }

  }
}