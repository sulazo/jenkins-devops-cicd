pipeline {
    agent any

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
    post{
        always{
            echo "i run always"
    }
    
    
    success {
            echo "i run when u are successful"
    
    } 
    failure{
        echo"i run when you err"
    }
    
 }


}