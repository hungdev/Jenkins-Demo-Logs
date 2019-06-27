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
                    for (commit in pullRequest.commits) {
                      echo "SHA: ${commit.sha}, Committer: ${commit.committer}, Commit Message: ${commit.message}"
                    }
                }
            }
        }
    }
}