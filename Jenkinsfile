pipeline {
    agent any
    options {
        buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '10')
    }
    environment {
        JENKINS_NODE_COOKIE= 'do_not_kill'
        CI='false'
    }
    stages {
        stage('git clone') {
            steps {
                git branch: 'main', credentialsId: 'f339a2ea-e49f-44df-86f8-a7f7229dfd26', url: 'https://github.com/adithya1150/test11.git'
            }
        }
        stage('starting api') {
            steps {
                sh 'ls'
                }
            }
        stage('git clone') {
            steps {
                git branch: 'master', credentialsId: 'f339a2ea-e49f-44df-86f8-a7f7229dfd26', url: 'https://github.com/adithya1150/test.git'
            }
        }
}
