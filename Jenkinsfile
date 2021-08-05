pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Stage'
                nodejs('node-16') {
                sh "npm install"
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage'
                nodejs('node-16') {
                sh "npm run test: integration"
                }
            }
        }
        stage('Integration') {
            steps {
                echo 'Integration Stage'
                sh cp . /var/www/
            }
        }
    }
}
