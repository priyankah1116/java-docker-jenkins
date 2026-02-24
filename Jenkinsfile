pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/priyankah1116/java-docker-jenkins.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t java-docker-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run --rm java-app'
            }
        }
    }
}
