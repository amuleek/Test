pipeline {
    agent any
    tools {
        maven 'Maven 3.6.3' // Ensure Maven is configured in Jenkins
        jdk 'JDK 11' // Ensure JDK is configured in Jenkins
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building Maven project for Development'
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests for Development'
                sh 'mvn test'
            }
        }
    }
}
