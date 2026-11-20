pipeline {
    agent { label 'linux' }

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Verify checkout') {
            steps {
                sh 'git log -1 --oneline'
            }
        }
    }
}
