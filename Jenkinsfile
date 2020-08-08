pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                withMaven(maven : 'Maven_Install' {
					sh 'mvn clean compile'
                }
            }
		}

        stage('Testing') {
            steps {
                withMaven(maven : 'Maven_Install' {
					sh 'mvn test'
                }
            }
		}

        stage('Deploy') {
            steps {
                withMaven(maven : 'Maven_Install' {
					sh 'mvn deploy'
                }
            }
		}
	}
}
