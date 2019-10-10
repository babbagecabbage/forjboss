pipeline {
    agent any

    stages {
        stage('create web archive') {
            steps {
                echo 'creating..'
                bat 'jar -cvf formcheck.war *' 
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying to standalone server ..'
                bat 'copy *.war "C:\\Naman\\EAP-7.2.0\\standalone\\deployments"' 
            }
        }
    }
}                  
