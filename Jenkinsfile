#!/usr/bin/env groovy
pipeline {
    agent none
    stages {
        stage('Build') {
            steps {
                sh "mvn package -Dmaven.test.skip=true"
            }
        }
    }
}
