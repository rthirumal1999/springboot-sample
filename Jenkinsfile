pipeline {
    agent any
    stages {
        stage('Build'){
            steps {
                gradle clean build -DskipTests
            }
        }
        stage('Test'){
            steps {
               gradle test
            }
        }
        stage('Deploy'){
            steps {
                gradle clean
            }
        }
    }
} 
