pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Task: Build, compile and package the application.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests and integration tests.'
                echo 'Tools: JUnit and Selenium'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse source code and check code quality.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Task: Scan the source code for security vulnerabilities.'
                echo 'Tool: Snyk'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy the application to the staging environment.'
                echo 'Tool: AWS EC2'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests in the staging environment.'
                echo 'Tool: Postman/Newman'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy the application to the production environment.'
                echo 'Tool: AWS EC2'
            }
        }
    }
}
