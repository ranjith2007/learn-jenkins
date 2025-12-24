pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        timeout(time: 20, unit: 'SECONDS')
        disableConcurrentBuilds()
    }
    stages {
        stage('Build') {
            steps {

            sh 'echo This is build'
            //sh 'sleep 20'

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
            deleteDir()
        }
        success {
            echo 'This section runs when pipeline success'
        }
        failure {
            echo 'This section runs when pipeline failure'
        }
    }
}