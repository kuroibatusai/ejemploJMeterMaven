pipeline {
    agent any

    stages {

        stage('Test Amazon Navegacion') {
            steps {
                sh '''
                    /Users/kuroi/Desktop/apache-maven-3.6.3/bin/mvn verify -Pperformance
                '''
            }
        }
    }
}