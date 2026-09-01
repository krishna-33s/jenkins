pipeline {
    agent {
        node {
            label "ROBOSHOP"
        }
    }
    environment {
        COURSE = "DevOps with AWS"
    }
    stages {
        stage("Build") {
            steps {
                script{
                    sh """
                        echo "Building..."
                        echo "Course name is ${COURSE}"
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