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
                }
            }
        }
    }
}
