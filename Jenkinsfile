pipeline {
    agent {
        docker { image 'hashicorp/terraform:light' }
    }
    stages {
        stage('Test') {
            steps {
                step{
                sh 'docker run --rm -it --name terraform -v $WORKSPACE -w $WORKSPACE hashicorp/terraform:light version'
                }
            }
        }
    }
}
