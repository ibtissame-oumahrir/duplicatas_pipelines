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
       stage('Checkout') {
            steps {
                script {
                    if (params.branch == 'master') {
                        sh 'echo "Login incorrect"'
                        error 'authentification failed !!'
                    } else if (params.branch == 'feature') {
                        sh 'echo "Bitbucket est indisponible" && exit 1'
                    }
                }
            }
        }
      
        stage('Config') {
          steps {
                script {
                    if (params.branch == 'master') {
                        error 'Erreur survenue lors de la vérification pour la branche master !!'
                    } else if (params.branch == 'feature') {
                        error 'Erreur survenue lors de la vérification pour la branche feature !!'
                    }
                }
            }
        }
        stage('Verify') {
             steps {
                script {
                    if (params.branch == 'master') {
                       error "error !!"
                    } else if (params.branch == 'feature') {
                       error "error !!"
                    }
                }
            }
        }
        stage('Package') {
            steps {
                script {
                    if (params.branch == 'master') {
                       error "error !!"
                    } else if (params.branch == 'feature') {
                       error "error !!"
                    }
                }
            }
        }
        stage('Publish') {
            steps {
                script {
                    if (params.branch == 'master') {
                      error "error !!"
                    } else if (params.branch == 'feature') {
                       error "error !!"
                    }
                }
            }
        }
    }
}

