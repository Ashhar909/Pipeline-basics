pipeline {
    agent {
        docker {
            image 'python:3.8' // Use an appropriate Python Docker image
        }
    }
    
    stages {
        stage('Checkout') {
            steps {
                git branch:'master', url:'https://github.com/Ashhar909/Pipeline-basics.git'
            }
        }
        
        stage('Run Python Script') {
            steps {
                script {
                    // Run the Python script
                    sh 'python hello.py'
                }
            }
        }
    }
    
    post {
        always {
            // Clean up or perform other actions if needed
        }
    }
}

