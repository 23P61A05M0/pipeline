pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/23P61A05M0/pipeline.git', branch: 'main'
            }
        }

        stage('Run Script') {
            steps {
                bat 'python python.py'
            }
        }
    }
}
