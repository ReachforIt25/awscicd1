pipeline {
    agent any

    stages {
        stage('git checkout'){
            steps{ 
                git branch: 'main', url: 'https://github.com/ReachforIt25/awscicd1.git'
            }
        }
        stage("test"){
            steps{
                sh "echo test"
            }
        }
    }
        
}


