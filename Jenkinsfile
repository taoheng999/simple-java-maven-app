pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        node {
          label 'docker'
        }

      }
      steps {
        sh 'sh \'mvn -B -DskipTests clean package\''
      }
    }

  }
}