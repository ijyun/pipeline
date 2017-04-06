pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        parallel(
          "hello": {
            echo 'hello'
            
          },
          "world": {
            echo 'world'
            
          }
        )
      }
    }
    stage('jenkins') {
      steps {
        echo 'jenkins'
      }
    }
  }
}