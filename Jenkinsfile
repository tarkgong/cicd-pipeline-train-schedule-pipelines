pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation -Dorg.gradle.java.home=/usr/local/java/jdk1.7.0_80'
                sh './gradlew build -Dorg.gradle.java.home=/usr/local/java/jdk1.7.0_80 --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}