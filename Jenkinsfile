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
                sh '''
                    set -e  # Detener el script si ocurre un error
                    cd /home/administrator/node-production
                    if [ ! -d "nueva-carpeta-desde-jenkins" ]; then
                        sudo mkdir nueva-carpeta-desde-jenkins
                    fi
                '''
            }
        }
    }
}