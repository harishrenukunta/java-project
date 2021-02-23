pipeline{
    agent any
    stages{
        stage('Clean, package java project'){
            steps{
                  sh 'mvn -DskipTests clean package'
            }
        }
        
        stage('Execute unit tests via maven'){
            steps{
                sh 'mvn test'
            }
        }
    }
}
