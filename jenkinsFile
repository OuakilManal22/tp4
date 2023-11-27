// Jenkinsfile

pipeline {
    agent any
    stages {
        stage('Cloning Git') {
            steps {
                git branch: 'main', url: 'https://github.com/OuakilManal22/tp4.git'
            }
        }
        stage('Building image') {
            steps {
                script {
                    echo 'Building image...'
                }
            }
        }

        stage('Test image') {
            steps {
                script {
                    echo 'Testing image...'
                }
            }
        }
        stage('Publish Image') {
            steps {
                script {
                    echo 'Publishing image...'
                }
            }
        }
    }

    post {
        success {
            echo 'Pipeline successful!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
