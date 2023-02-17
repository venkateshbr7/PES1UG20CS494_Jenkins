pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS494-1', wait: fal
                 echo 'Build by PES1UG20CS494 successful
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test by PES1UG20CS494 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by PES1UG20CS494 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
