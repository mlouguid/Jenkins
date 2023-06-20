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

        stage('script') {
          steps {
            sh 'dotnet build eSopOnWeb.sln'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'docker --version'
      }
    }

    stage('azure ') {
      steps {
        echo 'hello  azure'
      }
    }

  }
}