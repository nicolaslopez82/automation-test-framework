pipeline{
    agent{ docker { image 'maven:3.6-alpine'} }
    stages{
        stage('log version info'){
            steps{
                sh 'docker run --name jenkins -p 8080:8080 -p 50000:50000'
                sh '-v /var/run/docker.sock:/var/run/docker.sock'
                sh '-v $(which docker):/usr/bin/docker'
            }
        }
    }
}