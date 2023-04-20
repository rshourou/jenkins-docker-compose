pipeline {
    agent any
    stages {
        stage("Verify tooling") {
            steps {
                sh ''' 
                sudo docker info
                sudo docker version
                docker compose version
                curl --version
                jq --version
                '''
            }
        }
    }
}