pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                echo "hello world."
            }
        }

        stage('Versions') {
            steps {
                sh 'node --version'
                sh 'svn --version'
            }
        }
    }
}
