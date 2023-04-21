pipeline {
    agent {
        docker {image 'node:16-alpine'}
    }
    stages {
        stage("Verify tooling") {
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