pipeline {
    agent { label "master" }
    stages {
        stage('build') {
            steps {
                sh 'java -version'
                sh 'git-version'
            }
        }
    }
}
