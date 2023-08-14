#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:3.5.0'
               args "-u root"
        }
      }
      steps {
      	sh 'mvn clean install'
      }
    }
  }
}
