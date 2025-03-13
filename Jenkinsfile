pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling hello.cpp...'
                // Replace YOUR_SRN with your actual SRN value
                sh 'g++ hello.cpp -o PES2UG22CS441-1'
            }
        }
        stage('Test') {
            steps {
                echo 'Running the executable...'
                sh './PES2UG22CS441-1'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add your deployment commands here, if any
            }
        }
    }

    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
