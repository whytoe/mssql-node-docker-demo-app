pipeline {
  agent {
    docker {
      image 'hello-world'
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
    stage('Slack') {
      steps {
        dockerNode(image: 'hello-world', socket: true) {
          isUnix()
        }
        
      }
    }
  }
}