pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello, World from malek!'
            }
        }
    }
    stage('Sonarqube Analysis ') {
            steps {
                withSonarQubeEnv('sonarqube-10.6.0.'){
                sh 'mvn sonar:sonar'
                }
                }
            }
            
        }
}
