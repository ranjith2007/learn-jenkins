pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {

            sh 'echo This is build'

            }
        }
        stage('Test') {
            steps {

            sh 'echo This is Test'

            }
        }
        stage('Deploy') {
            steps {

            sh 'echo This is Deploy'

            }
        }
    }
    post {
        always  {
            echo 'This sections runs always'
        }
        success {
            echo 'This section runs when pipeline success'
        }
        failure {
            echo 'This section runs when pipeline failure'
        }
    }
}