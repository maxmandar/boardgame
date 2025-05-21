pipeline {
    agent any   // ✅ This tells Jenkins: run this pipeline on any available executor
    tools {
        maven 'maven3'
        jdk 'jdk17'
    }

    stages {     
        stage('Compile') {
            steps {
               sh "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
