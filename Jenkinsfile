pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/your-username/simple-website.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}

