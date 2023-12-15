pipeline {
    agent any
    tools {nodejs "node"}
    stages {
        stage('Checkout') {
			steps {
				checkout scm
			}
		}

        stage('Git') {
            steps {
                git 'git@github.com:ggraotech/angular-todo.git'
            }
        }
        
        stage('Build') {
            steps {
                sh 'npm install --legacy-peer-deps'
                sh 'npm run build -y'
            }
        }  
    }
}
