pipeline {
  agent any
  
  stages {
    stage('Build Image') {
      steps {
        script {
          withEnv(["PATH+DOCKER=${tool 'docker'}"]) {
            def image = docker.build("front-end:${env.BUILD_ID}")
          }
        }
      }
    }
  }
}
