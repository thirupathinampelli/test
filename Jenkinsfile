pipeline {
    agent any

    stages {
        stage('Install Seomthing') {
            steps {
                sh 'sudo apt install apache2 -y'
            }
        }
	stage('Get my code') {
            steps {
                git credentialsId: '72ae0822-4c0e-4b36-964c-cd06664558ff', url: 'https://github.com/pathakbhaskar/test.git'
            }
        }
	stage('Deploy') {
            steps {
                sh '''sudo cp -R * /var/www/html/
                    sudo chmod -R 777 /var/www/html/'''
            }
        }
    }
}
