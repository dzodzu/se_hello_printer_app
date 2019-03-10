pipeline {
    agent any
    stages {
	stage('Linter') {
	    steps {
		    sh 'make lint'
		}
	}
	stage ('Deps') {
	    steps {
		    sh 'make deps'
		}
	}
        stage('Test') {
            steps {
	            sh 'make test'
        	}
        }
    }
}
