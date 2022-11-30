pipeline {
    agent any

    stages {
        stage('Git Update') {
            steps {
                echo 'Git Update'
                git url: 'https://github.com/gowns764/test-repo.git', branch: 'main'
            }
        }
        stage('Test') {
            steps {
                sh "/usr/local/bin/kubectl get pod"
            }
        }
    }
}