pipeline {
    agent {
        node {
            label "ROBOSHOP"
        }
    }
    stages {
        stage("Build") {
            steps {
                script{
                    sh """
                        echo "Building..."
                        exit 1
                    """
                }
            }
        }
        stage("Test") {
            steps {
                script{
                    sh """
                        echo "Testing..."
                    """
                }
            }
        }
        stage("Deploy") {
            steps{
                script{
                    sh """
                        echo "Deploying..."
                    """
                }
            }
        }
    }

    post {
        always {
            echo "here it is hii hello"
        }
        success {
            echo "successfully completed"
        }
        failure {
            echo "failed"
        }
    }
}