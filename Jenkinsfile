pipeline{
    agent label: 'master'
    currentBuild{
        displayName = "${env.BRANCH_NAME} -> ${env.CHANGE_TARGET}"
    }
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
