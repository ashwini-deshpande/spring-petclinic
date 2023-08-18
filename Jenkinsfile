#!groovy
pipeline {
  agent {
    docker { image 'openjdk:17-alpine3.13' }
  }
  stages {
    stage('Maven Install') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
