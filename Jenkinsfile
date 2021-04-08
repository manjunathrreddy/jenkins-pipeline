pipeline {
    agent {
        docker { image 'hashicorp/terraform:light' }
    }
    stages {
        stage('Test') {
            steps {
                docker run --rm -it --name terraform -v $WORKSPACE -w $WORKSPACE hashicorp/terraform version
            }
        }
    }
}
