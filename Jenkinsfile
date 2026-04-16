pipeline {
    agent any

    tools {
        maven "Maven3"
        jdk "JDK17"
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Disha-L12/MyMavenWebApp.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Tomcat...'
            }
        }
    }
}
