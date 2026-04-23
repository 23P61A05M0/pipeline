pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')   // checks GitHub every 1 minute
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/23P61A05M0/pipeline.git'
            }
        }

        stage('Run Script') {
            steps {
                bat 'python python.py'
            }
        }
    }
}
