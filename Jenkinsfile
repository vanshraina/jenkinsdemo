pipeline {
    agent any

    tools {
        maven 'Maven-3.9'
    }

    triggers {
        githubPush()
    }

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/vanshraina/jenkinsdemo.git'
            }
        }

        stage('Build Project') {
            steps {
                bat 'mvn clean install'
            }
        }
    }
}
