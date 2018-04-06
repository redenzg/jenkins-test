#!/usr/bin/env groovy

node('master') {
    stage('say-hello') {
        sh "echo 'hello world'"
        sh "mkdir /home/jenkins/app"
        sh "cd /home/jenkins/app"
        sh "git clone https://github.com/redenzg/jenkins-test.git"
        sh "cd jenkins-test"
        sh "composer install"
    }
}
