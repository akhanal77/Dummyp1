pipeline {
    agent {
        docker {
            image 'adoptopenjdk:8u282-b08-jre-hotspot'
        }
    }
    triggers{
        pollSCM('* * * *  *')
    }
    parameters { 
        string(
            name: 'DEPLOY_ENV', 
            defaultValue: 'staging', 
            description: 'This will be param') 
    }
    stages {
        stage('Test Stage') {
            environment {CLASS_NAME='DEVOPS'}
            steps {
                sh 'java -version'
                sh 'echo $HOSTNAME'
                sh 'echo $CLASS_NAME'
            }
        }
    }
}
