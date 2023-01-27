pipeline {
    agent any

    stages {

        stage ('Build Docker Image') {
            scripts {
                dockerapp = docker.build("tpbsdocker/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
            }
        }
    }

}