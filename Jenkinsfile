pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'HTML Project Ready'
            }
        }
    }

    post {
        always {
            publishHTML(target: [
                reportDir: '.',
                reportFiles: 'index.html',
                reportName: 'My HTML Website',
                keepAll: true,
                allowMissing: false,
                alwaysLinkToLastBuild: true
            ])
        }
    }
}