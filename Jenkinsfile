pipeline { 
    agent {
        label "ws"
    }
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo ***** Starting Style checks *******"
                sh "npm i jslint"
                sh "/node_modules/jslint/bin/jslint.js server.js"
                sh "echo **** Starting Style checks *******"
            }
        }
        stage('Static Code Analysis') {
            steps {
                sh "echo Starting Static code analysis"
            }
        }
    }
}