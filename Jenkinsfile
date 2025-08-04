pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t image1 .'
            }
        }
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name bank-app -p 1111:80 shaikmustafa/paytm:bank'
            }
        }
    }
}
