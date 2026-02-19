pipeline {
    agent any
    parameters {
        string(name: 'MESSAGE', defaultValue: 'Hello from VS Code', description: 'Experiment 1 Message')
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Verification') {
            steps {
                echo "Task 2: The parameter value is: ${params.MESSAGE}"
                bat 'echo Task 3: Hello from Jenkins'
            }
        }
    }
}