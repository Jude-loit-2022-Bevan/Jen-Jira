pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Check python version') {
            steps {
                script {
                    sh "python --version"
                }
            }
        }

        stage('Run Python Code') {
            steps {
                script {
                    // Assuming your Python script is named 'main.py'
                    sh "python hello.py"
                }
            }
        }
    }

    // post {
    //     always {
    //         // Clean up or post-build actions can be added here
    //     }
    // }
}
