pipeline { 
agent any 

    tools{
        nodejs 'node-16'
    }

    stages { 
        stage ('Build') { 
            steps {
                echo 'This is Build stage'
                sh 'npm install'
            }
 
        }
        stage ('Test') { 
            steps {
                echo 'This is Test stage'
                sh 'npm run test:integration'
            }
        
        }
        stage ('Deploy') { 
            steps{
                echo 'This is Deploy stage'
            }
        }         
    }           
 }
