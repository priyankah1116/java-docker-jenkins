pipeline {
    agent any

    stages {
        stage('Show Files') {
            steps {
                sh 'ls -l'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t hello-java .'
            }
        }

        stage('Run Java App') {
            steps {
                sh 'docker run --rm hello-java'
            }
        }
    }
}
