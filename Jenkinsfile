pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  options {
    ansiColor('xterm')
  }

  parameters {
    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
  }

  environment {
    SAMPLE_URL="example.com"
  }

  stages {

    stage('One') {
      steps {
        sh 'echo Hello World'
        sh 'echo Hello Universe'
        sh 'echo ${SAMPLE_URL}'
        sh 'echo PERSON - ${PERSON}'
      }
    }

  }

  post {
    always {
      sh 'echo Post CleanUP steps'
    }
  }

}
