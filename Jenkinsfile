pipeline {
  agent any
  stages {
    stage ("stage 1") {
      steps {
        sh "pwd"
      }
    }
    stage ("stage 2") {
      steps {
        sh "date"
      }
    }
    stage ("stage 3") {
      steps {
        sh "ls"
      }
    }
  }
  post {
      always {
        // Archive test report
        echo "I will always run"
      }
      success {
        // Only if the test passes
        echo "Execution successfull"
      }
      failure {
        // If tests fails
        echo "Execution failed"
      }
    }
}