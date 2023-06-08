pipeline {
  agent none
  stages {
    stage('message') {
      parallel {
        stage('message') {
          steps {
            echo 'hello all'
            echo 'Bonjour tout le monde'
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