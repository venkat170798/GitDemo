pipeline {
    agent any

    stages {

        stage('SCM') {
            steps {
                git branch: 'webhook-demo',
                url: 'https://github.com/venkat170798/GitDemo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Done') {
            steps {
                echo 'Completed pipeline'
            }
        }
    }
}
