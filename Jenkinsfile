pipeline {
    agent {
        node {
            label "ROBOSHOP"
        }
    }
    environment {
        COURSE = "DevOps with AWS"
    }
    options {
        disableConcurrentBuilds()
        timeout(time: 5, unit: 'SECONDS')
    }
    stages {
        stage("Build") {
            steps {
                script{
                    sh """
                        echo "Building..."
                        echo "Course name is ${COURSE}"
                        sleep 10
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