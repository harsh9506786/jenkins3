pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/harsh9506786/jenkins3.git'
            }
        }
        stage('Run') {
            steps {
                bat 'node index.js'
                bat 'node index2.js'
            }
        }

         stage('Run2') {
            steps {
                bat 'node test.js'
            }
        }

        stage('Test') {
            steps {
                bat 'node test.js'
            }
        }
    }
}
