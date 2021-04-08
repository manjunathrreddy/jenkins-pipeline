pipeline {
    agent {
        docker { image 'hashicorp/terraform:light' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'terraform version'
            }
        }
    }
}
