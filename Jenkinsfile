pipeline {
    agent any
    tools {
        maven"maven1"
    }
     stages{
         stage('fetch'){
             steps{
                 echo'fetch maven project from github'
                 git branch:'main',
                 url:'https://github.com/gagansodhi/devoops.git'
         }
     }   
        
        stage('Maven Clean') {
            // Execute the clean goal of Maven
            sh 'mvn clean'
        }

        stage('Maven Validate') {
            // Execute the validate goal of Maven
            sh 'mvn validate'
        }

        stage('Maven Compile') {
            // Execute the compile goal of Maven
            sh 'mvn compile'
        }

        stage('Maven Test') {
            // Execute the test goal of Maven
            sh 'mvn test'
        }

        stage('Maven Package') {
            // Execute the package goal of Maven
            sh 'mvn package'
        }

        stage('Maven Verify') {
            // Execute the verify goal of Maven
            sh 'mvn verify'
        }

        stage('Maven Install') {
            // Execute the install goal of Maven
            sh 'mvn install'
        }

        stage('Maven Site') {
            // Execute the site goal of Maven
            sh 'mvn site'
        }

        stage('Maven Deploy') {
            // Execute the deploy goal of Maven
            sh 'mvn deploy'
        }
    } 
    } 
        stage('executing generate jar') {
            steps{
                echo 'executing the generate jar file'
                sh 'java -jar ./target/Sum.jar 20 30 15 50 72'
            }
        }
}
