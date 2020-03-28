pipeline {
    agent any

    stages {
        stage('Stage 1') {
            steps {
                echo "Stage 1 processing"
            }
        }
		 stage('Stage 2') {
            steps {
                echo "Stage 2 Processing"
            }
        
		stage('Stage 3') {
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
						echo "Stage 3.3 Processing"
					}
				}
			}
        }
		
    }
}