pipeline {
    agent any
    tools {
        maven 'maven-jenkins'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
