pipeline {
    agent any

    environment {
        FLUTTER_HOME = '/var/jenkins_home/development/flutter'
        PATH = "${env.FLUTTER_HOME}/bin:${env.PATH}"
    }

    stages {
        stage('Flutter Pub Get') {
            steps {
                sh 'flutter pub get'
            }
        }
        
        stage('Flutter Build Web') {
            steps {
                sh 'flutter build web'
            }
        }
    }
}
