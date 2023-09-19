pipeline {
    agent {
       label 'awsslave'
    }
    triggers {
        githubPush()
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh """
                   ls -l /home
                   sudo docker pull ubuntu
                   sudo docker images
                   test
                   """
            }
        }
        stage('Test') {
            steps {
                sh """
                   ls -l /home
                   sudo docker pull ubuntu
                   sudo docker images
                   """
            }
        }
        stage('Deploy') {
            steps {
                sh """
                   ls -l /home
                   sudo docker pull ubuntu
                   sudo docker images
                   """
            }
        }
    }
}
