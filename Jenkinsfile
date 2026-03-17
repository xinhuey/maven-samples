pipeline {
  agent any
  tools {
        maven 'maven1'
        jdk 'Java_25'
    }
  stages {
    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }

    stage('test') {
      steps {
        bat 'mvn test'
      }
    }

    stage('verify') {
      steps {
        bat 'mvn verify'
      }
    }

  }
  
}