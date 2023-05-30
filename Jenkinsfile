pipeline {
  agent any
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

  }
}