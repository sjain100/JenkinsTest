pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                withMaven(maven : 'maven_3_6_3' {
					sh 'mvn clean compile'
                }
            }
		}

        stage('Testing') {
            steps {
                withMaven(maven : 'maven_3_6_3' {
					sh 'mvn test'
                }
            }
		}

        stage('Deploy') {
            steps {
                withMaven(maven : 'maven_3_6_3' {
					sh 'mvn deploy'
                }
            }
		}
	}
}
