pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                withMaven(maven : 'Maven_Install' {
					sh 'mvn clean compile'
                }
            }
		}

	}
}
