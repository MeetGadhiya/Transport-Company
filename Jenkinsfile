pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }


	stage('Test') {
            steps {
                sh 'mvn test'
		echo 'New Test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }






        }
    }
}
