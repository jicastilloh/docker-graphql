pipeline{
    agent any
    stages{
        stage ('Build'){
            steps{
                echo 'Ejecutando etapa build'
            }
        }
        stage ('Tests'){
            steps{
                echo 'Ejecutando tests'
            }
        }
        stage ('Deploy'){
            steps{
                withCredentials([string(credentialsId: '9371d6e1-5d0f-4b99-9f7a-f63a0f762e4a', variable: 'SUDO_PASS')]) {
                    sh '''
                        set -e  # Detener el script si ocurre un error
                        cd /home/administrator/node-production
                        echo $SUDO_PASS | sudo -S mkdir -p nueva-carpeta-desde-jenkins
                    '''
                }
            }
        }
    }
}