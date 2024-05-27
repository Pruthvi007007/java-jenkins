pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Clean up any previously compiled files
                sh 'rm -rf build'
                
                // Create a build directory
                sh 'mkdir build'
                
                // Compile the Java code and move the compiled class file to the build directory
                sh 'javac -d build HelloWorld.java'
            }
        }
        stage('Test') {
            steps {
                // You can add commands to run tests here if you have any test suite
                // Example: sh 'java -cp build:lib/junit.jar org.junit.runner.JUnitCore MyTestClass'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the built Java application
                // For simplicity, just execute the compiled class file
                sh 'java -cp build HelloWorld'
            }
        }
    }
}
