#!/usr/bin/env groovy

node('master') {
    stage('say-hello') {
        sh "echo 'hello world'"
        sh "mkdir -p /home/jenkins/app"
        sh "cd /home/jenkins/app"
        sh "rm -rf /home/jenkins/app/jenkins-test && cd /home/jenkins/app && git clone https://github.com/redenzg/jenkins-test.git"
        sh "cd /home/jenkins/app/jenkins-test && composer install"
    }
}
