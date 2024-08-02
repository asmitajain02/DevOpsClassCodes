pipeline {
   agent any  
    tools {
        maven 'Maven'
    }

    stages {
        stage('Compile') {
            steps {
                sh "mvn compile"
            }
        }
        
        stage('UnitTesting'){
            steps {
                sh "mvn test"
            }
        }
        stage('Codecoverage'){
            steps {
               sh "mvn verify"  
            }
        }
        stage('Package'){
            steps {
               sh "mvn package"   
            }
        }
    }
}
