pipeline {
    agent {
        docker {
            image "node:22"
        }
    }
        timeout(time:1 , unit:'MINUTES')
    }
    stages{
        stage('inicio pipeline'){
            steps {
                sh 'echo "saludos desde jenkins en el terminal"'
            }
        }
                stage('dependencias'){
            steps {
                sh 'echo "instalando dependencias"'
                sh 'npm install'
            }
        }
        stage('fin pipeline'){
            steps {
                echo 'saludos desde jenkins en el pipeline'
            }
        }
    }

