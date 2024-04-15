pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                script {
                    echo "Checkout stage"
                   
                }
            }
        }
        
        stage('Compile Sources in Master Environment') {
            steps {
                script {
                    echo "Compile Sources in Master Environment stage"
          
                }
            }
        }
        
        stage('Verify Quality: Sonar') {
            steps {
                script {
                    echo "Verify Quality: Sonar stage"

                }
            }
        }
    }
}
