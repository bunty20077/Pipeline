/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'golang:1.19.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
    }
}
