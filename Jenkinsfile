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
    stage('error') {
      steps {
        parallel(
          "hi": {
            echo 'hi'
            
          },
          "ha": {
            echo 'ha'
            
          }
        )
      }
    }
    stage('end') {
      steps {
        echo 'end'
      }
    }
  }
}