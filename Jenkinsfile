pipeline {

    agent any

    tools {
        nodejs 'node_18'
    }
    
    stages {
	stage('Node-Version') {
            steps {
                sh 'npm version'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
                
            }
        }

	stage('Run') {
            steps {
                sh 'npm start'
            }
        }
    }
}