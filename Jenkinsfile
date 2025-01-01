pipeline {
    agent any
    stages {
        stage('Run Test.js in Docker') {
            steps {
                echo 'Running test.js inside Docker container...'
                sh 'docker run --rm -v $(pwd):/usr/src/app -w /usr/src/app node:16 node test.js'
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
