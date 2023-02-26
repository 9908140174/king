pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'this is unit test'
      }
    }

    stage('build') {
      steps {
        sh '''pwd
ls
cal 2023'''
      }
    }

    stage('testing') {
      parallel {
        stage('testing') {
          steps {
            echo 'this is test'
          }
        }

        stage('Qs check') {
          steps {
            echo 'QA cheking'
          }
        }

      }
    }

    stage('deploy-prod') {
      steps {
        echo 'deploy on prod'
      }
    }

  }
}