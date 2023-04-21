pipeline {
    agent none
    stages {
        stage("Verify tooling") {
            agent {
                docker {image 'node:16-alpine'}
            }       
            steps {
                sh 'node --version'
                sh ''' 
                sudo docker info
                sudo docker version
                sudo docker compose version
                curl --version
                jq --version
                '''
            }
        }
    }
}