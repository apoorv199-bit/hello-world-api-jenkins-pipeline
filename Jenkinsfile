pipeline {
    agent any

    environment {
        JAVA_HOME=tool 'jdk17'
        MAVEN_HOME=tool 'maven'
    }

    stages {
        stage("Build"){
            steps{
                sh 'mvn clean install'
            }
        }

        stage("Test"){
            steps{
                sh 'mvn test'
            }
        }
    }
}