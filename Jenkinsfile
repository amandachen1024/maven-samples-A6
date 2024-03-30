pipeline {
  agent any
  tools {
    maven 'Maven'
    jdk 'JDK'
  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/amandachen1024/maven-samples-A6.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn clean test verify'
      }
    }

  }
}
