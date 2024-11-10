pipeline {
    agent any
      stages {
        stage('Example'){
            steps {
                sh '''
                    env | grep -e PATH -e JAVA_HOME
                    which java 
                    java -version
                '''    
            }
        }
    }
}