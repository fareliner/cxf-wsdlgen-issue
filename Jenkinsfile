pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        def mvnv = 'mvn-3.5.0'
        withEnv( ["PATH+MAVEN=${tool mvnv}/bin"] ) {
          sh 'mvn --batch-mode -U clean install'
        }
      }
    }
  }
  environment {
    env = 'dev'
  }
}
