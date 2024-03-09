pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG21CS395-1.cpp -o temp'
                 build job: 'PES1UG21CS395-1', wait: false
                 echo 'Build by CS395 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG21CS395-1.cpp'
                echo 'Test by CS395 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS395 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
