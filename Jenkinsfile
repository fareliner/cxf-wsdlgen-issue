pipeline {
  agent any
  tools {
    maven 'apache-maven-3.5.0'
  }
  stages {
    stage('Build') {
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        sh 'mvn --batch-mode -U clean install'
      }
    }
  }
}
