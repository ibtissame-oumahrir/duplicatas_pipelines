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
             stage('Lecture du fichier CSV') {
            steps {
                script {
                    def csvFile = sh(script: "curl -sS https://github.com/ibtissame-oumahrir/duplicatas_pipelines/raw/db/errors.csv", returnStdout: true).trim()
                    def lines = csvFile.split('\n')
                    
                    for (line in lines) {
                        def fields = line.split(',"')
                        def pipelineType = fields[0].replaceAll('"', '')
                        def errors = fields[1].replaceAll('"', '')
                        
                        if (pipelineType == 'db') {
                            def errorMessages = errors.split('], ')
                            for (errorMessage in errorMessages) {
                                currentBuild.result = 'FAILURE'
                                error(errorMessage.replaceAll('[', '').replaceAll(']', ''))
                            }
                        }
                    }
                }
            }
        }
       stage('Checkout') {
            steps {
                script {
                    if (params.branch == 'master') {
                        // Simuler une erreur de login incorrect pour master
                        sh 'echo "Login incorrect"'
                        error 'authentification failed !!'
                    } else if (params.branch == 'feature') {
                        // Simuler une erreur indiquant que Bitbucket est indisponible pour feature
                        sh 'echo "Bitbucket est indisponible" && exit 1'
                    }
                }
            }
        }
      
        stage('Verify') {
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
        stage('Install Dev DB') {
             steps {
                script {
                    if (params.branch == 'master') {
                        error 'Unable to connect to DB, please contact your DBA administrator'
                    } else if (params.branch == 'feature') {
                        error 'Erreur survenue lors de la vérification pour la branche feature !!'
                    }
                }
            }
        }
        stage('Install Val DB') {
            steps {
                script {
                    if (params.branch == 'master') {
                        error 'Unable to connect to DB, please contact your DBA administrator'
                    } else if (params.branch == 'feature') {
                        error 'Erreur survenue lors de la vérification pour la branche feature !!'
                    }
                }
            }
        }
    }
}
