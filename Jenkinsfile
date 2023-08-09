pipeline {
    stages {
        stage('Checkout Git') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'Github-credential', url: 'https://github.com/Feng-HelloWorld/Multi-branch-pipeline.git']]])
            }
        }

        stage('Build') {
            steps {
                script {
                    sh "echo 'Hello World'"
                }
            }
        }
    }
}