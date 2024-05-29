pipeline {
    agent any
    tools {
        maven 'Maven 3.6.3' // Ensure Maven is configured in Jenkins
        
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building Maven project for QA'
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests for QA'
                sh 'mvn test'
            }
        }
    }
}
