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
                bat 'mvn clean test'
                bat 'mvn clean package'
            }
        }
        
        stage('Test') { 
            steps {
                // 
                echo 'Etape Test'
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
                bat 'copy 
            }
        }
    }
}
