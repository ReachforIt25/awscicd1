pipeline {
    agent any

    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/bilacando/awscicd.git'
        IMAGE_TAG = 'awscicd'
    }
    stages{
        stage('git checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }

        stage('docker build'){
            steps{
                sh 'docker build -t "${IMAGE_TAG}" .'
                sh 'docker images'

            }
        }
        
    }
}
