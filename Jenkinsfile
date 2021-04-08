pipeline {
    agent {
        docker { image 'terraform:light' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'terraform version'
            }
        }
    }
}


docker run -i -t hashicorp/terraform:light plan