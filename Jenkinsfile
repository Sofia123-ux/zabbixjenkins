pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'git@github.com:Sofia123-ux/zabbixjenkins.git', credentialsId: 'your-credentials-id'
            }
        }
        stage('Run Jenkinsfile') {
            steps {
                script {
                    // Run the Jenkinsfile from a specific folder
                    load 'ci/Jenkinsfile'
                }
            }
        }
    }
}
