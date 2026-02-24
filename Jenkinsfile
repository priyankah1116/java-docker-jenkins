pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/priyankah1116/project-jenkins.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t java-ci-cd .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run --rm java-ci-cd'
            }
        }
    }
}