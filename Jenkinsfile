pipeline {
    agent {
        docker {
            image 'node:14' 
            args '-p 3000:3000' 
        }
    }
    environment {
        npm_config_cache = 'npm-cache'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building'
                sh 'yarn install'
                sh 'yarn build'
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