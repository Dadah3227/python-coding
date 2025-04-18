pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Hi'){
            steps{
                echo 'Hi'
            }
        }
        state('Github checkout'){
            steps{
                git changelog: false, credentialsId: 'dadah_git_cred', poll: false, url: 'https://github.com/Dadah3227/python-coding.git'
                sh 'ls -ltr' // unix
             // bat 'dir' // windows
            }
        }
    }
}
