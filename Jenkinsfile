pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
                file_name="e.cpp"
                g++ $file_name -o $output_file
                
            }
        }
        
        stage('Test') {
            steps {
                sh 'echo "Testing..."'
                
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'echo "Deploying..."'
                
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline finished'
        }
        
        failure {
            echo 'Pipeline failed'
        }
    }
}
