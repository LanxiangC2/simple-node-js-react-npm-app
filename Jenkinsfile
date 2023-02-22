pipeline {
    agent {
        docker {
            image 'node' 
        }
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building'
                sh 'npm cache clean'
                sh 'npm --version'
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}