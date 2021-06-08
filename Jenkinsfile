pipeline {
    agent any

    stages {
        stage('Configure libraries') {
            steps {
                sh "sudo apt install apache2 -y"
                sh "sudo service apache2 start"
                echo 'Configured utilities'
            }
        }
        stage('Deploy') {
            steps {
                sh "cp index.html /var/www/html/"
                echo 'Deployed'
            }
        }
    }
}
