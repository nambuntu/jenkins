pipeline {
    agent any
    triggers {
        cron('H/5 * * * *')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}