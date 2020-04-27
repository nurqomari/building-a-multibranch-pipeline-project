pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
        stage("Post Build"){
            steps{
                echo "====++++executing Post Build++++===="
            }
            post{
                always{
                    echo "====++++always++++===="
                }
                success{
                    echo "====++++Post Build executed successfully++++===="
                }
                failure{
                    echo "====++++Post Build execution failed++++===="
                }
        
            }
        }
    }
}
