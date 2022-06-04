pipeline {
    tools {
        maven "maven-3.8.5"
    }
    agent any
    stages {
        stage('Fetch Code') {
            steps {
                git branch: 'paac', url: 'https://github.com/Emadmohamed22/Vprofile-Project.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}

