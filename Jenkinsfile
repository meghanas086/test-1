pipeline {
    agent any
    tools {
        jdk 'java-11'
        maven 'maven'
    }
    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/meghanas086/test-1.git'
            }
        }
        stage('Compile') {
            steps {
                sh "mvn -X compile"
            }
        }
        stage('Build') {
            steps {
                sh "mvn clean install"
            }
        }
    }
}
