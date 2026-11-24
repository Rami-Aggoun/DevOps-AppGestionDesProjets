
pipeline {
    agent any

    tools {
        jdk 'JDK21'
        maven 'Maven3'
    }

    stages {

        stage('Maven Compile') {
            steps {
                dir('backend') {
                    echo 'Starting Maven compilation...'
                    sh 'mvn clean compile'
                }
            }
        }

    }

    post {
        success {
            echo 'Maven compilation completed successfully!'
        }

        failure {
            echo 'Maven compilation failed!'
        }
    }
}
