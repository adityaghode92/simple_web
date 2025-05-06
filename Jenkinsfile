pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/my-website.git'
            }
        }
        stage('Clean Old Site') {
            steps {
                sh 'sudo rm -rf /var/www/html/*'
            }
        }
        stage('Deploy') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
