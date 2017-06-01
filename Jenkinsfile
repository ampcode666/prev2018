pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "error": {
            build 'mvn'
            
          },
          "": {
            timeout(time: 12)
            
          }
        )
      }
    }
  }
}