pipeline {
    agent any

    stages {
        stage('Print Python Code') {
            steps {
                sh 'cat hello.py'
            }
        }

        stage('Run Python Code') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}


