pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'develop', url: 'https://github.com/KevinCha1234/etl-Trabajo-Final-DataOpps.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python transform.py'
            }
        }

        stage('Ejecutar Lectura') {
            steps {
                sh 'python lecutra.py'
            }
        }   
    }
}
