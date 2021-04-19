pipeline {
    agent none
    stages {
        stage('Develop branch deploy to mixyznik.club') {
            agent { label 'remote-node-new' }
            when {
                expression { env.GIT_BRANCH == 'dev' }
            }
            steps {
                    echo "deploy to mixyznik.club started"
                    sh 'printenv'
                    sh 'pwd'
            }
        }
        stage('Master branch deploy to master') {
            agent { label 'master'}
            when {
                 branch "master"
            }
            steps {
                    echo "deploy to master started"
                    sh 'printenv'
                    sh 'pwd'
                 }
        }
    }
    }
