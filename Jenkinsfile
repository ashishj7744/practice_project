pipeline {
    agent any

    stages {

        stage('Deploy DEV') {
            when {
                branch 'dev1'
            }
            steps {
                sh '''
                cd /var/www/dev/practice_project
                git pull origin dev1
                '''
            }
        }

        stage('Deploy UAT') {
            when {
                branch 'uat1'
            }
            steps {
                sh '''
                cd /var/www/uat/practice_project
                git pull origin uat1
                '''
            }
        }

        stage('Deploy PROD') {
            when {
                branch 'prod1'
            }
            steps {
                sh '''
                cd /var/www/prod/practice_project
                git pull origin prod1
                '''
            }
        }
    }
}
