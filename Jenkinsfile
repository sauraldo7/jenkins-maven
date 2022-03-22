pipeline {
    agent any 
    stages {
        stage('compile and clean') { 
            steps {
		sh "echo hi this multibranch jenkins"               
                sh "mvn clean compile"
            }
        }
        stage('Test') { 
            steps {
                 sh "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                 sh "mvn package"
            }
        }
    }
}
