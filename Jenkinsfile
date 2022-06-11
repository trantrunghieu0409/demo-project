#!/usr/bin/env groovy
pipeline {
    agent any 
    stages {
        stage ('hello') {
            steps {
                echo 'HelloWorld'
            }
        }
        stage('build') {
            steps {
                javac 'HelloWorld.java'
                java 'HelloWorld'
            }
        }
        stage('testing') {
            steps {
                echo 'testing...'
                sleep 5
                echo 'test successfully'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploying...'
                sleep 2
                echo 'deployed'
            }
        }
    }
}