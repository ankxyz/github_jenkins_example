pipeline {
    agent { 
		docker { 
			image 'python:3.7-alpine'
			args '-u root:root'
		} 
    }
    stages {
        stage('build') {
            steps {
                sh 'pip install requests'
				sh 'pwd && ls'
				sh 'python app.py'
            }
        }
    }
}
