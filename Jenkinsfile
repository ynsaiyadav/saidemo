pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                git 'https://github.com/ynsaiyadav/saidemo.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
