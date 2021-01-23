pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "/Users/kuroi/Desktop/apache-maven-3.6.3/bin/mvn clean"
            }
        }

        stage('Compile') {
            steps {
                sh "/Users/kuroi/Desktop/apache-maven-3.6.3/bin/mvn compile"
            }
        }

        stage('Test2') {
            steps {
                sh '''
                    /Users/kuroi/Desktop/apache-maven-3.6.3/bin/mvn test
                '''
            }
        }

        stage('Test Amazon Navegacion') {
            steps {
                sh '''
                    /Users/kuroi/Desktop/apache-maven-3.6.3/bin/mvn verify -Pperformance
                '''
            }
        }
    }
}