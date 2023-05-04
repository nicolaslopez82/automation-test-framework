pipeline{
    agent{ docker { image 'maven:3.6-alpine'} }
    stages{
        stage('log version info'){
            steps{
                sh 'docker --version'
            }
        }
    }
}