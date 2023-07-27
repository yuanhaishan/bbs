pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/yuanhaishan/bbs.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        // stage('Test') {
        //     steps {
        //         sh 'mvn test'
        //     }
        // }
        // stage('Deploy') {
        //     steps {
        //         sh 'mvn deploy'
        //     }
        // }
    }
}
