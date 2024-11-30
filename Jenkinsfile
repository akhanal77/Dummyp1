pipeline {
    agent {
        docker { image 'hello-world:latest ' }
    }
    stages {
        stage('Test') {
            steps {
                echo Hello World
                //sh 'node --eval "console.log(process.platform,process.env.CI)"'
            }
        }
    }
}
