pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo "TAG BUILD_TAG.toLowerCase()"
                checkout scm
                sh 'ls -ltr'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo "env.BRANCH_NAME is the branch"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo "env"
            }
        }
    }
}
