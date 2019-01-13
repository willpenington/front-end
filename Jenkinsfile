pipeline {
  agent any
  
  stages {
    stage('Build Image') {
      steps {
        script {
          kubernetes.image().withName("example").build().fromPath(".")
          
        }
      }
    }
  }
}
