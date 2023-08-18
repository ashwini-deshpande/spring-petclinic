#!groovy
pipeline {
  agent {
    docker { image 'anapsix/alpine-java' }
  }
  stages {
    stage('Maven Install') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
