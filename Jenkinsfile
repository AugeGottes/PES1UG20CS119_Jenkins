pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS119-1 your_cpp_file.cpp'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES1UG20CS119-1'
            }
        }
        
        stage('Deploy') {
            steps {
                // Add deployment steps here
                echo 'Deploying....'
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed'
        }
        
        failure {
            echo 'Pipeline failed'
        }
    }
}
