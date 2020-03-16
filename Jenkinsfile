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
                echo 'DONE' 
            }
        }
        stage('Deploy') { 
            steps {
                echo 'DONE'
            }
        }
	}
}