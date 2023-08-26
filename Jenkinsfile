pipeline {

    agent {
        docker {
            image "${AGENT_BASE_IMAGE}"
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
                sh 'mvn native:compile-no-fork -P native'
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