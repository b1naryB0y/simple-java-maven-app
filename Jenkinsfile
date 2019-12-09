pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.ms:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B _DskipTests clean package'
            }
        }
    }
}
