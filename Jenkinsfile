pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh '''
                export PATH=/sbin:/usr/sbin:/usr/bin:/usr/local/bin

                newman run /Users/nehajain/Desktop/folder/runner.json -e/Users/nehajain/Desktop/folder/env.json
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
