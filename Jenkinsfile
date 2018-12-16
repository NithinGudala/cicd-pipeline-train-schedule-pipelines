pipeline {
    agent any
    stages {
        stage('Build') {
        when{
        brach 'master'
        }
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
