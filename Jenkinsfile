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
                    if (params.branch == 'master') {
                        error '[ERROR] COMPILATION ERROR :, [ERROR] Source option 5 is no longer supported. Use 7 or later., [ERROR] Target option 5 is no longer supported. Use 7 or later., [ERROR] Failed to execute goal org.apache.maven.plugins:maven-compiler-plugin:3.1:compile (default-compile) on project fornax-cartridges-sculptor-generator-35: Compilation failure: Compilation failure:, [ERROR] Source option 5 is no longer supported. Use 7 or later."'
                    } else if (params.branch == 'feature') {
                        error '174840 [main] [ERROR] COMPILATION ERROR :, 174840 [main] [ERROR] /app/home/prodjenkins/jenkins/workspace/BOPV32_pwc-api_bopv32_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/ConversionRateConverter.java:[15,19] cannot find symbol, 174840 [main] [ERROR] /app/home/prodjenkins/jenkins/workspace/BOPV32_pwc-api_bopv32_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/ConversionRateConverter.java:[20,61] cannot find symbol, 174840 [main] [ERROR] /app/home/prodjenkins/jenkins/workspace/BOPV32_pwc-api_bopv32_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/ConversionRateConverter.java:[38,9] cannot find symbol, 174840 [main] [ERROR] /app/home/prodjenkins/jenkins/workspace/BOPV32_pwc-api_bopv32_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/ConversionRateConverter.java:[37,12] cannot find symbol"'
                    }
                }
            }
        }
        
        stage('Build') {
            steps {
                script {
                    if (params.branch == 'master') {
                        error '607394 [main] [ERROR] COMPILATION ERROR :, 607395 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/HSBCIM_pwc-api_hsbcim_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/mapper/SetPDArrangementDetailsV35RqMapper.java:[10,19] cannot find symbol, 607395 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/HSBCIM_pwc-api_hsbcim_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/mapper/SetPDArrangementDetailsV35RqMapper.java:[30,5] cannot find symbol, 607395 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/HSBCIM_pwc-api_hsbcim_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/mapper/SetPDArrangementDetailsV35RqMapper.java:[40,9] cannot find symbol, 607395 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/HSBCIM_pwc-api_hsbcim_develop@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/impl/v2/SetPDArrangementDetailsWebService.java:[26,19] cannot find symbol'
                    } else if (params.branch == 'feature') {
                        error '137598 [main] [ERROR] COMPILATION ERROR :, 137598 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/BMCE_pwc-api_bmce_master@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/MerchantEquipmentContractConverter.java:[15,19] cannot find symbol, 137598 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/BMCE_pwc-api_bmce_master@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/MerchantEquipmentContractConverter.java:[20,72] cannot find symbol, 137598 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/BMCE_pwc-api_bmce_master@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/MerchantEquipmentContractConverter.java:[40,9] cannot find symbol, 137598 [main] [ERROR] /app/home/prodjenkins/.jenkins/workspace/BMCE_pwc-api_bmce_master@2/ws-core-impl/src/generated/java/com/acp/vision/pcrd/ws/converter/MerchantEquipmentContractConverter.java:[38,12] cannot find symbol'
                    }
                }
            }
        }
        
        stage('Configure && Build') {
         steps {
                script {
                    if (params.branch == 'master') {
                        error '3266 [main] [ERROR] Failed to execute goal org.apache.maven.plugins:maven-deploy-plugin:2.8.2:deploy (default-deploy) on project PowerCardConnectApi: Failed to deploy artifacts: Could not transfer artifact ma.hps.pwc35.pluton.ws.dbshk.master:PowerCardConnectApi:ear:3.5.2-d5747 from/to pwc35-maven-releases (http://10.1.90.11:8081/nexus/repository/pwc35-maven-releases/): Failed to transfer file: http://10.1.90.11:8081/nexus/repository/pwc35-maven-releases/ma/hps/pwc35/pluton/ws/dbshk/master/PowerCardConnectApi/3.5.2-d5747/PowerCardConnectApi-3.5.2-d5747.ear. Return code is: 405, ReasonPhrase: Method Not Allowed. -> [Help 1], 3266 [main] [ERROR], 3266 [main] [ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch., 3266 [main] [ERROR] Re-run Maven using the -X switch to enable full debug logging., 3266 [main] [ERROR]"'
                    } else if (params.branch == 'feature') {
                        error 'Erreur survenue lors de la vérification pour la branche feature !!'
                    }
                }
            }
        }
        
        stage('Publish to Nexus') {
           steps {
                script {
                    if (params.branch == 'master') {
                        error '23159 [main] [ERROR] Unable to create temporary files, 23173 [main] [ERROR] Unable to continue dependency-check analysis., 23723 [main] [ERROR] Failed to execute goal org.owasp:dependency-check-maven:5.3.2:check (default) on project PwcWSGateway: Fatal exception(s) analyzing PwcWSGateway: One or more exceptions occurred during analysis:, 23724 [main] [ERROR] 	Unable to create temporary files, 23724 [main] [ERROR] 	No documents exist"
                             api,"3791 [main] [ERROR] Failed to execute goal org.apache.maven.plugins:maven-deploy-plugin:2.8.2:deploy (default-deploy) on project PowerCardConnectApi: Failed to deploy artifacts: Could not transfer artifact ma.hps.pwc35.pluton.ws.sib.develop:PowerCardConnectApi:ear:3.5.4-a0605-20240401.064318-1 from/to pwc35-maven-snapshots (http://10.1.90.11:8081/nexus/repository/pwc35-maven-snapshots/): Failed to transfer file: http://10.1.90.11:8081/nexus/repository/pwc35-maven-snapshots/ma/hps/pwc35/pluton/ws/sib/develop/PowerCardConnectApi/3.5.4-a0605-SNAPSHOT/PowerCardConnectApi-3.5.4-a0605-20240401.064318-1.ear. Return code is: 405, ReasonPhrase: Method Not Allowed. -> [Help 1], 3798 [main] [ERROR], 3798 [main] [ERROR], 3798 [main] [ERROR] For more information about the errors and possible solutions, please read the following articles:, 3798 [main] [ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoExecutionException"'
                    } else if (params.branch == 'feature') {
                        error '2805 [main] [ERROR] Failed to execute goal org.apache.maven.plugins:maven-deploy-plugin:2.8.2:deploy (default-deploy) on project PowerCardConnectApi: Failed to deploy artifacts: Could not transfer artifact ma.hps.pwc35.pluton.ws.utb.master:PowerCardConnectApi:ear:3.5.4-a065c from/to pwc35-maven-releases (http://10.1.90.11:8081/nexus/repository/pwc35-maven-releases/): Failed to transfer file: http://10.1.90.11:8081/nexus/repository/pwc35-maven-releases/ma/hps/pwc35/pluton/ws/utb/master/PowerCardConnectApi/3.5.4-a065c/PowerCardConnectApi-3.5.4-a065c.ear. Return code is: 405, ReasonPhrase: Method Not Allowed. -> [Help 1], 2805 [main] [ERROR], 2805 [main] [ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch., 2805 [main] [ERROR] Re-run Maven using the -X switch to enable full debug logging., 2805 [main] [ERROR]'
                    }
                }
            }
        }
         
    }
}
