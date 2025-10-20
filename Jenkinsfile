pipeline {
    agent any   // Run on any available Jenkins agent

    stages {
        stage('Checkout') {
            steps {
                echo "Cloning the GitHub repository..."
                git 'https://github.com/sravandskdevops/Git.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                sh 'mvn clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying the application..."
                sh 'echo Application deployed successfully!'
            }
        }
    }
}

