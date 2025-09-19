pipeline {
  agent any
  stages {
    stage("stage 1") {
      steps {
        bat "cd"
      }
    }
    stage("stage 2") {
      steps {
        bat "date /t && time /t"
      }
    }
    stage("stage 3") {
      steps {
        bat "dir"
      }
    }
  }
  post {
    always {
      echo "I will always run"
    }
    success {
      echo "Execution successful"
    }
    failure {
      echo "Execution failed"
    }
  }
}
