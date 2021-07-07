pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'git branch: \'main\', credentialsId: \'credGithub\', url: \'https://github.com/IsraelNoah/test-nodejs-app.git\''
          }
        }

        stage('Run') {
          steps {
            echo 'Run reussit'
          }
        }

      }
    }

  }
}