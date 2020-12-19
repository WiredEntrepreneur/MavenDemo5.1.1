pipeline {
    agent any
    tools {
        maven 'my_mvn'
    }
    stages {
        stage("Checkout") {   
            steps {      
                       git branch: 'main',url: 'https://github.com/WiredEntrepreneur/MavenDemo5.1.1.git'
                }    
        }
        stage('Build') {
            steps {
            sh "mvn compile"       
            }
        }
        
        stage("Unit test") {               
            steps {       
                sh "mvn test"               
           }
            
        }
        
    }
}