pipeline {
    agent any

    stages {
        stage('Build') {                        
            steps {
                echo 'Building..'
                sleep {
                    time: 3
                    unit: seconds
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