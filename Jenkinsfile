pipeline {

    agent {
        docker {
            image 'maven:3-eclipse-temurin-17-alpine'
        }
    }

    stages {

        stage("Maven Build"){
            steps {
                sh 'mvn clean install'
            }
        }

        stage("Build binary"){
            steps {
                sh 'native:compile-no-fork'
            }
        }

        stage("Compress binary"){
            steps {
                echo 'To be implemented...'
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