pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /Users/taifu/.m2:/Users/taifu/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
