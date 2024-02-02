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
                sh 'npm install'
                sh 'react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res'
            }
        }
    }
}
