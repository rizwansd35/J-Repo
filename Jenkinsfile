pipeline {
    agent any
    
    environment {
               PATH = /opt/maven-3/bin:bin$PATH
    }

    stages {
        stage('Git Checkout') {
            steps {
                echo "git branch: 'main', url: 'https://github.com/rizwansd35/J-Repo.git'"
            } 
        }
        stage("Maven Build") {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
