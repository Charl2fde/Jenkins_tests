pipeline {
  agent {
    docker {
      image 'maven:3.9.5-amazoncorretto-17'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean '
        sh 'mvn compile'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }

  }
}