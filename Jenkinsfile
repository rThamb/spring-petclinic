pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				bat './mvnw package'
			}
		}
		stage('Test') { 
            steps {
                echo 'TEST' 
            }
        }
        stage('Package') { 
            steps {
                echo 'PACKAGE'
            }
        }
		stage('Deploy') { 
            steps {
                echo 'DEPLOY'
            }
        }
	}
}