pipeline {
    agent any
    tools (nodejs "nodejs")

    stages {
        stage('Build') {
            steps {
                git 'git@github.com:ggraotech/angular-todo.git'
                sh 'npm install'
            }
        }
    }
}
