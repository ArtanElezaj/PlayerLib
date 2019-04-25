pipeline {
    agent any
    tools {
     maven 'M3'
    }
    stages {
        stage('Checkout'){
            steps{
                git 'https://github.com/ArtanElezaj/PlayerLib.git'
            }
        }

        stage('Build'){
            steps{
                sh 'mvn clean compile'
            }
        }

        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }
    }
}