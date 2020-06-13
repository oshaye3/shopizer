pipeline {
    agent {
        docker {
            image 'dminds-shopizer:1.0'
            args '-v $HOME/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'docker pull moshaye/dminds-shopizer'
            }
        }
    }
}

