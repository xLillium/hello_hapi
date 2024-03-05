#!/usr/bin/env groovy

pipeline {

    agent {
        any {
            image 'node'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'npm test'
            }
        }
    }
}
