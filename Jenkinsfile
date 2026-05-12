pipeline {
    agent any

    environment {
        Python = 'C:\\Users\\Vaibhav\\AppData\\Local\\Programs\\Python\\Python314\\python.exe'
    }

    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Show Python Version') {
            steps {
                bat "${env.Python} --version"
            }
        }

        stage('Run extract.py') {
            steps {
                bat "${env.Python} extract.py"
            }
        }
    }
}