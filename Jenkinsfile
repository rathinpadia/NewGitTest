pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Stage 1 processing"
            }
        }
		 stage('Test') {
            steps {
                echo "Stage 2 Processing"
            }
		}
        
		stage('Deploy') {
			parallel{
				stage('Stage 3.1') {
					steps {
						echo "Stage 3.1 Processing"
					}
				}
				stage('Stage 3.2') {
					steps {
						echo "Stage 3.2 Processing"
					}
				}
				stage('Stage 3.3') {
					steps {
						echo "Stage 3.3 Processing changes with git checkin3"
					}
				}
			}
        }
		
    }
}