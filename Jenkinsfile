pipeline {
  agent any
  
  stages {
    stage('Build Image') {
      steps {
        script {
          docker.withTool("docker") {
            def image = docker.build("front-end:${env.BUILD_ID}")
          }
        }
      }
    }
  }
}
