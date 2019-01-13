pipeline {
  agent any
  stages {
    stage('Build Image') {
      steps {
        script {
          def image = docker.build("front-end:${env.BUILD_ID}")
        }
      }
    }
  }
}
