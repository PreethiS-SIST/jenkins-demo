pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Starting Build'
                sh 'pwd'
                sh 'ls'
                echo 'Build completed'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging application'
                sh 'mvn clean package'
                echo 'Package completed'
            }
        }
        stage('Deploy') {
    steps {
        sh 'cp target/jenkins-demo-1.0-SNAPSHOT.jar /opt/jenkins-demo/'
    }
}

    }
}
