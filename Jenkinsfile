pipeline {

    agent any

    tools {
        maven 'Maven 3.9.4'
    }

    stages {

        stage("Maven Build"){
            steps {
                sh 'mvn clean install'
            }
        }

        stage("Docker Build"){
            steps {
                echo 'To be implemented...'
            }
        }

        stage("Docker Login"){
            steps {
                echo 'To be implemented...'
            }
        }

        stage("Docker Push"){
            steps {
                echo 'To be implemented...'
            }
        }

    }

}