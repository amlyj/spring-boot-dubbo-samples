pipeline {
  agent {
    docker {
      image 'maven:3.6.2-jdk-8'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'mvn package -Dmaven.javadoc.skip=true -V -B'
      }
    }
  }
}