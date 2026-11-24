pipeline {
    agent any

    tools {
        jdk 'JDK21'
        maven 'Maven3'
    }

    stages {

        stage('Maven Compile') {
            steps {
                echo 'Starting Maven compilation...'
                sh 'mvn clean compile'
            }
        }

    }
}
