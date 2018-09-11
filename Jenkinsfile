pipeline {
    agent any
    options {
        timestamps()
    }
    stages {
        stage('Clear working directory') {
            steps {
                ansiColor('xterm') {
                    deleteDir()
                }
            }
        }
        stage('Configure') {
            steps {
                ansiColor('xterm') {
                    sh 'env > environment'
                }
            }
        }
    }
}
