pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                checkout scm
                sh 'mvn clean package'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
        stage('UnitTest') {
            steps {
                sh 'echo "Hello World"'
            }
        }
    }
}
