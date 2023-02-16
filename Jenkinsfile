pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
                sh 'g++ "main/hello1.cpp"' 
                
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
        
        failure {
            echo "Pipeline failed"
        }
    }
}
