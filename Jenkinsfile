pipeline {  
    agent any
    
    stages {
        stage('Construir') {  
            steps {  
                sh ' docker build -t hello-word-php-apache .'
                sh ' docker run -p 81:80 hello-word-php-apache '
            }
        }
        stage('Probar') {
            steps {
                sh ' wget http://localhost '
            }
        }
        
    }
}  