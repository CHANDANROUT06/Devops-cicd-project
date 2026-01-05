pipeline {
    agent any

    stages {

        stage('Clone Repo') {
            steps {
                echo 'Code already cloned by Jenkins'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-web .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh '''
                docker rm -f devops-web-container || true
                docker run -d -p 8081:80 --name devops-web-container devops-web
                '''
            }
        }
    }
}



