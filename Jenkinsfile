pipeline {
    agent { docker { image 'python:3.14.0a7-alpine3.21' } }
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