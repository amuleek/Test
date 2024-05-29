pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'Maven 3.6.3') {
                    sh 'mvn clean compile'
                }
            }
        }
    }
    
}
