pipeline {
    agent any
    tools { jdk 'JDK17' }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Aditya-Solunke23/hello-java-jenkins.git'
            }
        }

        stage('Compile Java') {
            steps {
                bat '''
                javac HelloWorld.java
                '''
            }
        }

        stage('Run Program') {
            steps {
                bat '''
                java HelloWorld
                '''
            }
        }
    }
}
