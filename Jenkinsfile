pipeline {
    agent { label 'linux' } 
    options {
        buildDiscarder(logRotator(numToKeepStr: '5'))
    }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
