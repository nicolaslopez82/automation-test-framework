pipeline{
    agent{ docker { image 'maven:3.6-alpine'} }
    stages{
        stage('log version info'){
            steps{
                sh 'grep docker /etc/group # GID
                    docker run  -p 8080:8080 -p 50000:50000 -d -u jenkins:GID  --name myjenkins jenkins:lst'
            }
        }
    }
}