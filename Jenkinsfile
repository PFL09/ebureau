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
                 bat 'mvn clean package'
            }
        }
        
         stage('deploy') { 
            steps {
                // 
                echo 'Etape Deploy'
                bat "copy /y 'target\\ebureau.war'  'C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps' "
               
               
            }
        }
    }
}
