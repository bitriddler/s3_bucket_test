
pipeline {
    agent any

    environment {
        AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
    }

    stages {
        stage('Build') {
            steps {
                sh "aws s3api list-buckets"
            }
        }
        stage('Preparation') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deployment') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
