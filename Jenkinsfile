pipeline {
    agent any
    stages {
        stage ('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/S-Vilka/InClassAssignmmentWeek6.git'
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
    post {
        success {
            echo 'Build was successful!'
        }
        failure {
            echo 'Build failed. Check logs for errors.'
        }
    }
}
