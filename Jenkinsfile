pipeline {
    agent {
        docker {
            image 'maven:3.9.11-eclipse-temurin-24'
        }
    }

    stages {
        stage("clean and compile") {
            steps {
                sh "mvn clean compile"
            }
        }

        stage("run test") {
            steps {
                sh "mvn test"
            }
        }
    }
}
