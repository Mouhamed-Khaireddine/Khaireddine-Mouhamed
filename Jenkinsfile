pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Mouhamed-Khaireddine/Khaireddine-Mouhamed.git'
            }
        }

        stage('Build Maven') {
            steps {
                dir('backend') {
                    sh 'mvn compile'
                }
            }
        }
    }
}
