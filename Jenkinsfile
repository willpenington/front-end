pipeline {
  agent any
  
  stages {
    stage('Build Image') {
      steps {
        script {
          kubernetes.image().withName("example").build().fromPath(".")
          #docker.withTool("docker") {
          #  def image = docker.build("front-end:${env.BUILD_ID}")
          #}
        }
      }
    }
  }
}
