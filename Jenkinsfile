pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'make'
                sh './addition'
            }
        }
    }
}
