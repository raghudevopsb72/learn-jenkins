pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  stages {

    stage('One') {
      steps {
        sh 'echo Hello World'
        sh 'echo Hello Universe'
      }
    }

  }

  post {
    always {
      sh 'echo Post CleanUP steps'
    }
  }

}
