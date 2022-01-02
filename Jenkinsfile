pipeline {
    agent { label 'linux' } 
    options {
        buildDiscarder(logRotator(numToKeepStr: '5'))
    }
    stages {
        stage('Scan') {
          steps {
            withSonarQubeEnv(installationName: 'sq1') { 
              sh './mvnw clean 'node:16.13.1-alpine'
            }
          }
        }
    }
}
