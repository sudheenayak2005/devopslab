pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
               git branch: 'main', url: 'https://github.com/sudheenayak2005/devopslab.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Static HTML project - no build needed'
            }
        }

        stage('Deploy') {
            steps {
               bat 'xcopy /E /Y * C:\xampp\htdocs\'
            }
        }
    }
}