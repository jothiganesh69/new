pipeline {
    agent any
    stages {
        stage('Version 1: Env Vars') {
            steps {
                // Task 1: Checkout
                checkout scm

                // Task 2: Print all Jenkins environment variables
                // In Windows, 'set' lists all variables
                bat 'set'

                // Task 3: Display custom echo message using specific variables
                echo "Custom Message: This is build #${env.BUILD_NUMBER} for the job ${env.JOB_NAME}"
            }
        }
    }
}
