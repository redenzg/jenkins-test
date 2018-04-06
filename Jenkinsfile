#!/usr/bin/env groovy

node('master') {
    stage('say-hello') {
        sh "echo 'hello world'"
        sh "git clone https://github.com/redenzg/jenkins-test.git"
        sh "composer install"
    }
}
