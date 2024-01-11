pipeline 
agent any   
        stage('Build') {
            steps {
                // Build your Java application using Maven
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run your tests
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy your application (e.g., copy artifacts to a server)
                // This is just a placeholder, actual deployment steps depend on your application and infrastructure
                echo 'Deploying the application...'
            }
        }
    }

    post {
        success {
            // This block will be executed if the pipeline succeeds
            echo 'Pipeline succeeded! Trigger further actions here.'
        }

        failure {
            // This block will be executed if the pipeline fails
            echo 'Pipeline failed! Handle failure scenarios here.'
        }
    }
}
