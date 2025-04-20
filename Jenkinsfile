pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Hello world'
          }
        }

        stage('Pre-Test') {
          steps {
            sleep 5
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sleep 5
      }
    }

  }
}