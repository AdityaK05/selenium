pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch:'main',url:'https://github.com/AdityaK05/selenium.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Selenium Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Custom Message') {
            steps {
                echo 'Selenium Automation Testing Executed Successfully!'
            }
        }

    }

