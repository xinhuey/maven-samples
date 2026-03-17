pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/xinhuey/maven-samples.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn clean compile test verify'
      }
    }

  }
  environment {
    maven = 'maven1'
    jdk = 'Java_25'
  }
}