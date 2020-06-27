#!groovy

pipeline {
  agent none
  stages {
    stage('Maven Install') {
      steps {
        bat "mvn clean install -Dmaven.test.skip=true"
      }
    }
    stage('Run tests') {
      agent any
      steps {
        bat "mvn test"
      }
    }
  }
}
