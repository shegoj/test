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
    		echo "${env.PATH}";
    		echo "${env.GIT_BRANCH}";
    		echo "${env.GIT_URL}";
    		echo "${env.JAVA_HOME}";
    		echo "${env.NODE_NAME}";
    		echo "${env.JOB_NAME}";
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo "${env}"
            }
        }
   }
}
