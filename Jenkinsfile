pipeline {
    agent any

    

    stages {
        stage('Build') {
            steps {
                echo 'Build'
                 sh 'npm install'
            }
        }

        stage('Push') {
            steps {
                echo 'Push'

              sh 'aws s3 sync dist/angular.demo/ s3://naga1122/'
            }
        }
}
}
