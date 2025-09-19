pipeline {
  agent any
  stages {
    stage ("stage 1") {
      steps {
        bat "cd"
      }
    }
    stage ("stage 2") {
      steps {
        bat "date /t"
      }
    }
    stage ("stage 3") {
      steps {
        bat "dir"
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
