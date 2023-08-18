#!groovy
pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'maven:3.8.3-openjdk-17' }
      }
      steps {
        sh '''
          mvn --version
          git --version
          mvn clean install
        '''
      }
    }
    stage('Front-end') {
      agent {
        docker { image 'node:16-alpine' }
      }
      steps {
        sh 'node --version'
      }
    }
  }
}
