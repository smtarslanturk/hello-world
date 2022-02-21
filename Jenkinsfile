pipeline {
    agent any
    environment { workdir = '/var/tmp/'}
    stages {
        stage('Env-Path')
            steps{
                echo "Env Var Path: ${env.workdir}"
            }
        stage('Build') {
            steps {
                echo "Application building step ..."
            }
        }
        stage('Test') {
            steps {
                echo "Testing stage ..."
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying stage ..."
            }
        }
    }
    post {
        always {
	        echo "Pipeline finished from post side"
        }
    }
}