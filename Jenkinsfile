pipeline {
    agent any

    stages {

        stage('Build Tier Two') {                        

            when { branch 'master' }

            steps {
                echo 'Building..'
                sleep(5) {
                    echo 'Waiting for 5 seconds'
                }
                echo 'Built completed in 5 seconds'
            }        

        }

        stage('Test') {
            
            when { branch 'master' }

            steps {
                echo 'Testing..'
            }

        }

        stage('Deploy') {

            when { branch 'master' }

            steps {
                echo 'Deploying....'
            }

        }

    }

}