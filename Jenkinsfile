pipeline {
    agent { docker { image 'python:3.13.3-alpine3.21' } }
    triggers {
        pollSCM 'H/1 * * * *'
    }
    stages {
        stage('build') {
            steps {
                sh 'python HelloWorld.py'
            }
        }
    }
}