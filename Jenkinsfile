pipeline {
    agent {
        docker {
            image 'gradle:8.7-jdk21-jammy'
            args '--user root -v $HOME/.gradle:/home/gradle/.gradle'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'gradle --version'
                sh 'gradle build'
            }
        }
    }
}