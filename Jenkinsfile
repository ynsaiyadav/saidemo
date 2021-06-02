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
        stage('archive'){
            steps{
                archiveArtifacts artifacts: 'project/target/*.war', followSymlinks: false
            }
        }
    }
}
