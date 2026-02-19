pipeline {
    agent any
    parameters {
        // Task 2: Accept USERNAME parameter from user
        string(name: 'USERNAME', defaultValue: 'John Doe', description: 'Enter your name to store in the file')
    }
    stages {
        stage('Version 4: User Persistence') {
            steps {
                // Task 1: Checkout latest version
                checkout scm
                echo "TASK 1: Checkout complete for Version 4."

                // Task 2 & 3: Create user.txt and store the parameter inside it
                echo "TASK 2: Captured Username: ${params.USERNAME}"
                
                // Using double quotes " " in bat allows Jenkins to swap ${params.USERNAME} with your input
                bat "echo ${params.USERNAME} > user.txt"
                echo "TASK 3: Username has been saved to user.txt."

                // Verify by displaying the file content
                echo "Verifying file content:"
                bat 'type user.txt'
            }
        }
    }
}
