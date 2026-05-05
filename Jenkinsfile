pipeline {
    agent any

    options {
        timestamps()
    }

    stages {
        stage('Build and test') {
            steps {
                sh 'mvn -B -ntp clean verify'
            }
        }
    }
}
