pipeline {
    agent {
        docker {
            image 'gradle:8.7-jdk21-alpine'  // 包含 Gradle + JDK 21
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'gradle --version'        // 验证 Gradle
                sh 'gradle build'           // 执行构建
            }
        }
    }
}