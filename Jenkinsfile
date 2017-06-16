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
        slackSend(message: 'The Build works', baseUrl: 'https://ops-sdc.slack.com', channel: '#development', teamDomain: 'ops-sdc', tokenCredentialId: 'OPS SDC Slack')
      }
    }
  }
}