pipeline {
    agent any
    tools {
            maven 'M3'
    }
    stages {
        stage('Build') { 
            steps {
                // 
                echo 'Etape compile'
                bat 'mvn clean compile'
                
                
            }
        }
        
        stage('Test') { 
            steps {
                // 
                echo 'Etape Test'
                bat 'mvn clean test'
            }
        }
        
        stage('Package') { 
            steps {
                // 
                echo 'Etape Packaging'
            }
        }
        
         stage('deploy') { 
            steps {
                // 
                echo 'Etape Deploy'
                bat 'mvn clean package'
               
            }
        }
    }
}
