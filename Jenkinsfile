pipeline {
    agent any
    
    
    stages {
        stage('Checkout') {
            steps {
                script {
                
                            sh 'echo "login incorrect !!  && exit 1 "'
                              sh 'echo "Login incorrect"'
                     
            }
            }  
        } 
        stage('Verify') {
            steps {
                script {
                
                        sh 'echo "Erreur lors de l\'exécution des tests de vérification"'
                  
                }
            }
        }
        
        stage('Install Dev DB') {
            steps {
                script { 
                        sh 'echo "Installation réussie de la base de données de développement"'
                }
            }
        }
        
        stage('Install Val DB') {
            steps {
                script {
                  
                        sh 'echo "Installation réussie de la base de données de validation"'
                   
            }
        }
    }
}
}

