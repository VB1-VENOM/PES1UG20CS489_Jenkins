pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
                sh 'g++ "main/hello.cpp"' 
                
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
            sh 'echo "Pipeline finished"'
        }
        
        failure {
            sh 'echo "Pipeline failed"'
        }
    }
}
