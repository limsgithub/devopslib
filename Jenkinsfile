#!groovy
pipeline {
    agent {
        node {
            label "master"
        }
    }
    stages {
        stage("build"){
            steps {
                script{
                    mvnHome = tool "M2"
                    sh "${mvnHome}/bin/mvn -v"
                    
                    nodeHome = tool "NODE"
                    sh "${nodeHome}/bin/node -v"
                    
                    goHome = tool "GO"
                    sh "${goHome}/bin/go -v"
                }
            }
        }
    }
}
