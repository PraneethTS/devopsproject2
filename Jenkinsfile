pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
     stage('Build') {
	steps{
		echo 'Running build automation'
		sh './gradlew -v'
	     }
	}
    }
}
