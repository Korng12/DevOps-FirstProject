pipeline {
    agent any

    stages {

        stage('Prepare') {
            steps {
                sh 'mkdir -p bin'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac -d bin src/*.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java -cp bin App'
            }
        }

    }
}