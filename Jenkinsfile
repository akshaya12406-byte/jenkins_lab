pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/akshaya12406-byte/Medical_recommender_System.git'
            }
        }
        stage('Build') {
            steps {
                // Change "sh" to "bat" for Windows!
                bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Change "sh" to "bat" for Windows!
                bat 'mvn test'
            }
        }
    }
}