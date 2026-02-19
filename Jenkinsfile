pipeline {
    agent any
    stages {
        stage('Version 3: File Operations') {
            steps {
                // Task 1: Checkout latest commit
                checkout scm
                echo "TASK 1: Latest code checked out."

                // Task 2: Create a file named output.txt using BAT
                // The '>' symbol redirects the echo text into a file
                bat 'echo This file was created by Jenkins Experiment 1 Version 3 > output.txt'
                echo "TASK 2: output.txt has been created."

                // Task 3: Display the contents of output.txt in console
                // 'type' is the Windows command to read file content
                echo "TASK 3: Reading file contents..."
                bat 'type output.txt'
            }
        }
    }
}
