pipeline {
   agent any
    tools {
        maven 'Maven 3.6.3' // Ensure Maven is configured in Jenkins
      }
   triggers {
        githubPush()
    }
  stages {
    stage('Test') {
      steps {
        sh '''
          node --version
          git --version
          curl --version
        '''
      }
    }
  }
}
