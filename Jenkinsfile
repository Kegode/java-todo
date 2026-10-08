pipeline{
    agent any
    tools{
        gradle "gradle"
    }
    stages{
        stage('clone code'){
            steps{
                git branch: "master", url: "https://github.com/Kegode/java-todo.git"
            }
        }
        stage('build code'){
            steps{
                sh "gradle build"
            }
        }
        stage('test code'){
            steps{
                sh "gradle test"
            }
        }
        stage('deploy code'){
            steps{
                echo 'deploying code'
            }
        }
    }
}