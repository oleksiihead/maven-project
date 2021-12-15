pipeline {
    agent any
    tools {
        maven 'maven-jenkins'
        dockerTool 'docker-jenkins'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
                sh "docker build -t tomcatwebapp:${env.BUILD_ID} ."
            }
        }
    }
}
