pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'javac Test.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java Test'
            }
        }
    }

    post {
        success {
            echo 'Build and Run stages completed successfully.'
        }
        failure {
            echo 'Build or Run stage failed.'
        }
        always {
            echo 'Pipeline finished.'
        }
    }
}
