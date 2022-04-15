pipeline {
   // agent any
   agent{docker{
	   image 'maven:3.6.3'
   }}

    stages {
        stage('Download') {
            steps {
                echo 'Continuous download'
            }
        }
        
         stage('Build') {
            steps {
                echo 'Continuos Build'
            }
        }
           stage('Test') {
            steps {
                echo 'Continuos testing ..'
            }
        }
           stage('Integration Test') {
            steps {
                echo 'Integration testing ..'
            }
        }
        
        
    }
    post{ //used tto clean up after building
        always{
            echo "i run always"
    }
    
    
    success {
            echo "i run when u are successful"
    
    } 
    failure{
        echo"i run when you err"
    }
	//changed{}
    
 }


}