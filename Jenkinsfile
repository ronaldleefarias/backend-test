pipeline {
    agent {
        docker {
            image "node:22"
        }
    }
    options {
        timeout(time:1 , unit:'MINUTES')
    }
    stages{
        stage('inicio pipeline'){
            steps {
                sh 'echo "iniciando pipeline"'
            }
        }
        stage('dependencias'){
            steps {
                sh 'echo "instalando dependencias"'
                sh 'npm install'
            }
        }
         stage('ejecutando test y coverage'){
            steps {
                sh 'echo "haciendo testiong al codigo"'
                sh 'npm run test:cov'
            }
        }
                 stage('ejecutando build'){
            steps {
                sh 'echo "haciendo build del codigo"'
                sh 'npm run build'
            }
        }
        stage('fin pipeline'){
            steps {
                echo 'finalizando pipeline'
            }
        }
    }
}