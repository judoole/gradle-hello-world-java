pipeline{
    agent label: 'master'
    stages{
        stage('Checkout'){
            steps{
                checkout scm
            }
        }
        stage('Assemble'){
            steps{
                sh 'echo hallois'
            }
        }
        stage('Unit tests'){
            steps{
                sh 'echo hei'
            }
        }
    }
}
