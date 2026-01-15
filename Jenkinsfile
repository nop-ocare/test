pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker compose build'
            }
        }
        stage('Test') {
             steps {
                 echo 'Running tests...'
                 sh 'npm test -- --run'
                 echo 'Tests completed.'
             }
        }
    }
}
