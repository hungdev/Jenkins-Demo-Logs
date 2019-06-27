import groovy.json.*
pipeline {
    agent any
    environment {
        PROJECT_NAME = 'Shoubotenken-Fontend'
    }
    stages {
        stage('First') {
            steps {
                script {
                    echo pullRequest
                }
            }
        }
    }
}