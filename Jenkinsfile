pipeline {
    agent any
    parameters {
        string(name: 'MESSAGE', defaultValue: 'Running Version 2', description: 'Enter message')
    }
    stages {
        stage('Version 2') {
            steps {
                // Task 1: Checkout (Explicitly shown)
                checkout scm
                echo "TASK 1: Source code successfully pulled from GitHub."

                // Task 2: Display System Date
                echo "TASK 2: Displaying System Date..."
                bat 'date /t'

                // Task 3: Print Parameter again
                echo "TASK 3: Parameter verification: ${params.MESSAGE}"
            }
        }
    }
}
