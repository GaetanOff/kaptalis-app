pipeline {
    agent any

    environment {
        PATH = "/opt/maven/bin:${env.PATH}"
    }

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
