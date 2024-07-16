pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'chmod +x ./build.sh'
                sh './build.sh'
            }
        }
        stage('Test') {
            steps {
                sh 'chmod +x ./testing.sh'
                sh './testing.sh'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cat ./deploy.sh'
                sh 'echo "Deploying..."'
                sh 'mv testfile.txt /tmp'
                sh 'ls -l /tmp'
            }
        }
    }
}