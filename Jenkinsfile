pipeline {
    agent any
    stages {
        stage("Verify tooling") {
            steps {
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