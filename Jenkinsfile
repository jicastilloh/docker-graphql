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
                sh 'pwd'
                sh 'cd /home/administrator/node-production'
                sh 'mkdir nueva-carpeta-desde-jenkins'
            }
        }
    }
}