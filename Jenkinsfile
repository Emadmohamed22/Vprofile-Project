pipeline {
    agent any
    stages {
        stage('Fetch Code') {
            steps {
                git branch: 'paac', url: 'https://github.com/Emadmohamed22/Vprofile-Project.git'
            }
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}
