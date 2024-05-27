pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Compile the Java code
                sh 'javac HelloWorld.java'
            }
        }
        stage('Test') {
            steps {
                // Run any tests (if you have)
                // You can add test commands here if you have any test suite
                // Example: sh 'java -cp .:junit.jar org.junit.runner.JUnitCore MyTestClass'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the built Java application
                // For simplicity, let's just execute the compiled class file
                sh 'java HelloWorld'
            }
        }
    }
}
