pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/harsh9506786/jenkins3.git'
            }
        }
        stage('Run') {
            steps {
                sh 'node index.js'
            }
        }
        stage('Test') {
            steps {
                sh 'node test.js'
            }
        }
    }
}
