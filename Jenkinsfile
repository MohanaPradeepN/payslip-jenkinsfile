pipeline {
    agent any 
    tools {
        maven 'maven' 
    }
    stages {
        stage('BUILD') {
            steps {
                build 'payslip-source'
            }
        }
        stage('TEST'){
            steps{
                build 'first-test'
            }
        }
        stage('DEPLOY'){
            steps{
                build 'first-build'
                build 'first-deploy'
            }
        }
    }
}
        
