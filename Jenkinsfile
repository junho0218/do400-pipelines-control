pipeline {
    agent {
        node {
            label 'nodejs'
        }
    }
    stages {
        stage('Backend Tests') {
            steps {
                sh 'node ./backend/test.js'
            }
        }
        steps {
            stage('Frontend Tests') {
                sh 'node ./frontend/test.js'
            }
        }
    }
}
