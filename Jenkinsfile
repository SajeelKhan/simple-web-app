pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Stage'
                sh "npm i"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage'
                sh "npm run test: integration"
            }
        }
        stage('Integration') {
            steps {
                echo 'Integration Stage'
                sh "git merge env.BRANCH_NAME"
            }
        }
    }
}
