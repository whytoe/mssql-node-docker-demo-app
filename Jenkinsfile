pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }
    
  }
  stages {
    stage('Test') {
      steps {
        echo 'Test my pipe'
      }
    }
    stage('Configure') {
      steps {
        sh 'ls'
      }
    }
  }
}