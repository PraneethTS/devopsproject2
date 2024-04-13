pipeline {
    agent any
    stages {
	stage('runtest'){
		steps{
			echo "helloo"
		}
        stage('Build') {
            steps {
                echo 'Running build automation'
		sh './gradlew -v'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        
    }
}
