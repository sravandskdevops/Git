pipeline {
    agent any    // Run on any available Jenkins agent (node)

    stages {

        stage('Checkout') {
            steps {
                echo "📦 Step 1: Checking out code from GitHub..."
                git branch: 'main', url: 'https://github.com/sravandskdevops/github.git'
            }
        }

        stage('Build') {
            steps {
                echo "🏗️ Step 2: Simulating build process..."
                sh 'echo Building project...'
                sh 'mkdir -p build && echo "Build successful" > build/output.txt'
            }
        }

        stage('Test') {
            steps {
                echo "🧪 Step 3: Running sample tests..."
                sh 'echo Running tests... && echo Tests passed!'
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Step 4: Deploying application..."
                sh 'echo Application deployed successfully!'
            }
        }
    }
}
