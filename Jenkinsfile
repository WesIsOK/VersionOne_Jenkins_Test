#!groovy

import groovy.json.JsonOutput
import groovy.io.FileType

node {
 properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('* * * * *')])])
 checkout scm

 stage('Start - Build env') {
    sh 'sudo ./script.sh'
 }

}
