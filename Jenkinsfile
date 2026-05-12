pipeline
agent any
environment {
    Python = 'C:\Users\Vaibhav\AppData\Local\Programs\Python\Python314\python.exe
'
}
stages {
    stage ('checkout Code') {
        
        steps {
            checkout scm    
        }
        stage ('show python version') {
            steps {
                bat "${env.Python} --version"
            }
            stage ('Run extract.py') {
                steps {
                    bat "${env.Python} extract.py"
                }
            }
        }
}