pipeline {
    agent any

    stages {

        stage ('Buil Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("p4ul0/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }
}