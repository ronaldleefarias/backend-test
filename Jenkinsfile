pipeline {
    agent any
    options {
        timeout(time:1 , unit:'MINUTES')
    }
    stages{
        stage('inicio pipeline'){
            steps {
                sh 'echo "saludos desde jenkins en el terminal"'
            }
        }
        stage('fin pipeline'){
            steps {
                echo 'saludos desde jenkins en el pipeline'
            }
        }
    }
}