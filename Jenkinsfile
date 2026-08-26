pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application from Git...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running automated tests...'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    mkdir -p "$HOME/Deployments/DemoApp"
                    cp index.html "$HOME/Deployments/DemoApp/index.html"
                    echo "Application deployed successfully."
                '''
            }
        }
    }
}
