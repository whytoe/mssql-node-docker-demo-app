pipeline {
  agent any
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
        slackSend(message: 'The Build works', channel: '#development', teamDomain: 'ops-sdc', token: 'Uoh9bLc1agibcxbUbkUOjoNU')
      }
    }
  }
}