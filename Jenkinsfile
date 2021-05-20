pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker {
          image '\'maven:3.8.1-adoptopenjdk-11\''
        }

      }
      steps {
        sh 'sh \'mvn --version\''
      }
    }

    stage('Front-end') {
      agent {
        docker {
          image 'image \'node:14-alpine\''
        }

      }
      steps {
        sh 'sh \'node --version\''
      }
    }

  }
}