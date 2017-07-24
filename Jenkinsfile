#!groovy

import groovy.json.JsonOutput
import groovy.io.FileType

node {
 properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('* * * * *')])])
 checkout scm

 stage('Start - Build env') {
    sh 'sudo I am an error'
    sh 'echo I am not the master branch'
    sh 'chmod a+x ./script.sh'
    sh './script.sh'
 }

}
