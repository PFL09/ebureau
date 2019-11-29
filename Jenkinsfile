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
                bat 'mvm clean compile'
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
            }
        }
    }
}
