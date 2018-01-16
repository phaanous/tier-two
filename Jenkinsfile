pipeline {
    agent any

    parameters {
        booleanParam(name: 'DO_BUILD', defaultValue: false, description: 'Will be bassed by integration job')
    }

    stages {

        stage('Build Tier Two') {                        
            when { 
                anyOf {
                    environment name: 'FEATURE_BUILD', value: true
                    branch: 'master'
                }
            }

            steps {
                echo 'Building..'
                sleep(3) {
                    echo 'Waiting for 3 seconds'
                }
                echo 'Built completed in 3 seconds'
            }        
        }

        stage('Test') {

            when { 
                anyOf {
                    environment name: 'FEATURE_BUILD', value: true
                    branch: 'master'
                }
            }

            steps {
                echo 'Testing..'
            }
        }

        stage('Deploy') {

            when { 
                anyOf {
                    environment name: 'FEATURE_BUILD', value: true
                    branch: 'master'
                }
            }

            steps {
                echo 'Deploying....'
            }
        }
    }
}