pipeline {
  agent none
  stages {
    stage('message') {
      steps {
        echo 'hello all'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'docker --version'
          }
        }

        stage('docker') {
          steps {
            sh 'docker ps'
          }
        }

      }
    }

    stage('azure ') {
      steps {
        echo 'hello  azure'
      }
    }

  }
}