pipeline {
    agent none
    
    parameters {
        string(name: 'x', defaultValue: 'date', description: 'cmd to execute : ')
    }

    stages {
        stage('Checkout') {
            agent any
            steps {
                sh "${params.x}"
                echo "Hello from main branch"
            }
        }
        stage('Build') {
            agent any
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            agent any
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            agent any
            steps {
                echo 'Deploying'
            }
        }
    }
}
