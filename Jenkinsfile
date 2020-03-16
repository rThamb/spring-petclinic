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
	post {
        success {
        mail to: 'omega180pro@gmail.com',
             subject: "The Pipeline Was Built Successfully: ${currentBuild.fullDisplayName}",
             body: "BUILD, TEST, PACKAGE, DEPLOY ran sucessfully. Visit ${env.BUILD_URL} for more info."
		}
	}
}