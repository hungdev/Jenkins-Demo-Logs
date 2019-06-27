import groovy.json.*
pipeline {
    agent any
    environment {
        PROJECT_NAME = 'Shoubotenken-Fontend'
    }
    stages {
        stage('First') {
            when {
                changeRequest()
            }
            steps {
                script {
                  echo "zzzzz: ${env.CHANGE_ID}"
                  if (env.CHANGE_ID) {
                    for (commit in pullRequest.commits) {
                      echo "hih"
                      // echo "SHA: ${commit.sha}, Committer: ${commit.committer}, Commit Message: ${commit.message}"
                    }
                    }
                }
            }
        }
    }
}