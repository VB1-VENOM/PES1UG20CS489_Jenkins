pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
                file_name="check.cpp"
                sh 'g++ $file_name' 
                
            }
        }
        
        stage('Test') {
            steps {
                sh 'echo "Testing..."'
                sh './a.out'
                
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
