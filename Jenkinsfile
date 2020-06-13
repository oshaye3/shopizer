pipeline {
    agent {
        docker {
            image 'dminds-shopizer'
            args '-v $HOME/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'sudo docker pull dminds-shopizer:1.0'
            }
        }
    }
}

