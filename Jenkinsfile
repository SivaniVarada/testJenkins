pipeline
{
    agent
    {
        docker {image 'node:16-alpine'}
    }
    stages
    {
        stage('test stage')
        {
            steps
            {
                sh 'node test.js'
                sh 'echo hiii!!'
            }
        }
    }
}