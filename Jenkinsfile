pipeline {
    agent any

    stages {
        stage('docker build') {
            steps {
                sh 'docker build -t react1:v1 .'
            }
        }
      stage('docker tag') {
            steps {
                sh 'docker tag react1:v1 prasadchandu/java:react-v1'
            }
        }
      stage('docker login') {
            steps {
                sh 'docker login'
            }
        }
      stage('docker push') {
            steps {
                sh 'docker push prasadchandu/java:react-v1'
            }
        }
    }
}
