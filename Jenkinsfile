pipeline {
    agent any
    tools{
        jdk 'java-11'
        maven 'maven'
    }
    stages{
        stage('git checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/meghanas086/test-1.git'
            }
        }
        stage('compile'){
            steps{
                sh "mvn compile"
            }
        }
       

    }
}
