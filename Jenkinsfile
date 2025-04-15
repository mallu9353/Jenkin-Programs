pipeline{
    agent any

    stages{
        stage('Build') {
            steps {
                sh 'javac Test.java'
            }
        }
        stage('Run'){
            steps {
                sh 'java Test'
        }

    }
}
}