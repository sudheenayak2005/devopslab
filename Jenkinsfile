pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/sudheenayak2005/devopslab.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Static HTML project - no build needed'
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}