pipeline {
    agent any
    
    stages {
        stage('Declarative') {
            steps {
                script {
                    echo "Declarative stage"
                }
            }
        }
        
        stage('Checkout SCM') {
            steps {
                script {
                    echo "Checkout SCM stage"
                }
            }
        }
        
        stage('Build') {
            steps {
                script {
                    echo "Build stage"
                }
            }
        }
        
        stage('Configure && Build') {
            steps {
                script {
                    echo "Configure && Build stage"
                }
            }
        }
        
        stage('Publish to Nexus') {
            steps {
                script {
                    echo "Publish to Nexus stage"
                }
            }
        }
    }
}
