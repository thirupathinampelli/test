pipeline {
    agent any

    stages {
        stage('Configure libraries') {
            steps {
                sh "install.sh"
                echo 'Configured utilities'
            }
        }
        stage('Deploy') {
            steps {
                sh "cp index.html /var/www/html/"
                echo 'Installed'
            }
        }
    }
}
