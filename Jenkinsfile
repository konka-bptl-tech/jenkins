pipeline {
    agent{
        label 'siva'
    }
     environment {
        JAVA_HOME = "/usr/lib/jvm/java-1.8.0-amazon-corretto.x86_64"
        PATH = "${JAVA_HOME}/bin:${env.PATH}"
    }
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Java Version'){
            steps{
                sh 'java -version'
            }
        }
        stage('Debug Env') {
            steps {
                sh 'env'
            }
        }
        stage('git version'){
            steps{
                sh 'git --version'
            }
        }
        stage('maven version'){
            steps{
                sh 'mvn --version'
            }
        }
        stage('Docker version'){
            steps{
                sh 'docker version'
            }
        }
        stage('trivy version'){
            steps{
                sh 'trivy version'
            }
        }
    }
}
