pipeline {
    agent any
        tool name: 'jenkins-terraform', type: 'terraform'
    stages {
        stage('Checkout the code') {
            steps {
                
                git branch: 'main', credentialsId: 'a8a9752e-f044-4f38-b8e7-9e9fab70b7a2', url: 'https://github.com/manjunathrreddy/jenkins-pipeline.git'
                
            }
        }
        stage('Print the version') {
            steps {
                
                sh 'terraform version'
                
            }

        }
    }
}
