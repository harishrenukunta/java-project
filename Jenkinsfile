pipeline{
    agent any
    stages{
        stage('Clean, package java project'){
            sh 'mvn -DskipTests clean package'
        }
        
        stage('Execute unit tests via maven'){
            sh 'mvn test'
        }
    }
}
