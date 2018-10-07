pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                checkout scm
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too. I know."
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
