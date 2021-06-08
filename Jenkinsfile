pipeline {
    agent any

    stages {
        stage('Configure libraries') {
            steps {
                sh "wget https://github.com/pathakbhaskar/test.git -O install.sh"
                sh "install.sh"
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
