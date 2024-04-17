
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
                        sh 'echo "Maximum checkout retry attempts reached, aborting"'
                            error "Checkout failed !!"
                    } else if (params.branch == 'feature') {
                        sh 'Please make sure you have the correct access rights'
                         error "Checkout failed !!"
                    }
                }
            }
        }
      
        stage('Compile Sources in Master Environment') {
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
        stage('Verify Quality: Sonar') {
             steps {
                script {
                    if (params.branch == 'master') {
                        error "Checkout failed !!"
                    } else if (params.branch == 'feature') {
                        error "Checkout failed !!"
                    }
                }
            }
        }
    }
}
