import groovy.json.*
pipeline {
    agent any
    environment {
        PROJECT_NAME = 'Demoo'
    }
    stages {
        stage('First') {
            // when {
            //     changeRequest()
            // }
            steps {
              sh "echo auth: ${env.CHANGE_AUTHOR}"
              sh "echo display name: ${env.CHANGE_AUTHOR_DISPLAY_NAME}"
              sh "echo branch: ${env.CHANGE_BRANCH}"
              sh "echo change id: ${env.CHANGE_ID}"
              sh "echo target: ${env.CHANGE_TARGET}"
              sh "echo title: ${env.CHANGE_TITLE}"
              sh "echo url: ${env.CHANGE_URL}"
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