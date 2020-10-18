#!groovy

pipeline {
  agent any
  stages {
    stage('Maven Install') {
      steps {
        bat "mvn clean install -Dmaven.test.skip=true"
      }
    }
    stage('Run tests') {
      steps {
        bat "mvn test"
      }
    }
  }
}
