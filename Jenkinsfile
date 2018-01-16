pipeline {
    agent any

    stages {
        stage('Build Tier Two') {                        
            steps {
                echo 'Building..'
                sleep(3) {
                    echo 'Waiting for 3 seconds'
                }
                echo 'Built completed in 3 seconds'
            }        
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}