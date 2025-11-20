pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out repository...'
                checkout scm
            }
        }

        stage('Run Commands') {
            steps {
                echo 'Running pipeline commands...'
                // Example shell command
                sh 'echo "Hello from Ubuntu VM!"'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished!'
        }
    }
}
