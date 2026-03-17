pipeline {
  agent any
  tools {
        maven 'maven1'
        jdk 'Java_25'
    }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/xinhuey/maven-samples.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        bat 'mvn clean compile test verify'
      }
    }

  }
  
}