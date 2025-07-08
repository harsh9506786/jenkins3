pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main' , url: 'https://github.com/harsh9506786/jenkins3.git'
            }
        }

        stage('Run') {
            steps {
                bat 'node index.js'
            }
        }

        stage('Test') {
            steps {
                bat 'node test.js'
            }
        }

       stage('Deploy') {
            steps {
                bat 'if not exist "C:\\deploy-folder" mkdir "C:\\deploy-folder"'
                bat 'copy index.js "C:\\deploy-folder\\"'
                bat 'copy index2.js "C:\\deploy-folder\\"'
                bat 'copy index.html "C:\\deploy-folder\\"'
    }
}

    }
}
