properties([
    parameters([
        choice(
            choices: ['master', 'feature'],
            description: 'Select a branch to build first',
            name: 'branch'
        )
    ])
])

pipeline {
    agent any
    
    stages {
        stage('Declarative: Checkout SCM') {
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
         stage('Deploy to Develop Environment') {
            steps {
                script {
                    echo "Declarative stage"
                }
            }
        }
    }
}
