pipeline {
    agent any

    stages {

        stage('Start Pipeline') {
            steps {
                echo 'Starting My Website CI/CD Pipeline'
            }
        }

        stage('Checkout') {
            steps {
                echo 'GitHub source code checked out successfully'
            }
        }

        stage('Verify Website Files') {
            steps {
                sh 'ls -l'
            }
        }

        stage('Validate HTML') {
            steps {
                sh 'test -s index.html'
                echo 'HTML file validation successful'
            }
        }
    }

    post {
        success {
            echo 'Website Pipeline Completed Successfully!'
        }

        failure {
            echo 'Website Pipeline Failed!'
        }
    }
}
