pipeline {
    agent any
    tools {
        maven 'Maven 3.6.3' // Ensure Maven is configured in Jenkins
       
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building Maven project for Production'
                sh 'mvn clean install'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to Production'
                sh 'mvn deploy'
            }
        }
    
