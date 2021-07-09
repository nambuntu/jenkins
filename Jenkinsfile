String cronString = env.BRANCH_NAME == "master" ? "*/2 * * * *" : ""

pipeline {
    agent any
    triggers {
        cron(cronString)
    }
    stages {
        stage('Example') {
            steps {
                echo cronString
                echo 'Hello World'
            }
        }
    }
    cronString = ""
    echo "cronString: " + cronString
}