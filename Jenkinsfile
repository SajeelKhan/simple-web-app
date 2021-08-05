pipeline {
    agent any

    tools{
        nodejs 'node-16'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building Stage'
                //sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage'
                //sh 'npm run test: integration'
            }
        }
        stage('Integration') {
            steps {
                echo 'Integration Stage'
                //sh cp . /var/www/
            }
        }
    }
}
