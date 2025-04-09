cat <<EOF > Jenkinsfile
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Cloning the repo..."
                checkout scm
            }
        }

        stage('Run Script') {
            steps {
                echo "Running hello.py"
                sh 'python3 hello.py'
            }
        }
    }

    post {
        success {
            echo "Build completed successfully ✅"
        }
        failure {
            echo "Build failed ❌"
        }
    }
}
EOF

