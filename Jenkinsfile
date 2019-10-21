pipeline {
         agent any
         tools {
                  maven 'Maven 3.6'
                  jdk 'JDK11'
         }
         stages {
         // your solution
                  stage('Compile') {
                           echo 'compiling...'
                           sh 'mvn compile'
                  }
                  stage('Unit Test') {
                           echo 'Unit Testing...'
                           sh 'mvn resources:testResources'
                           sh 'mvn compiler:testCompile'
                           sh 'mvn surefire:test'
                  }
         }
}
