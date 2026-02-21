pipeline {
    agent any

    tools {
        maven 'Maven-3.9'
    }

    triggers {
        pollSCM('H/1 * * * *')
    }

    stages {
        stage('Build Project') {
            steps {
                bat 'mvn clean install'
            }
        }
    }
}
