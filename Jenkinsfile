#!groovy

import groovy.json.JsonOutput
import groovy.io.FileType

node {
 properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('* * * * *')])])
 checkout scm

 stage('Start - Build env') {
    sh 'echo I am not the master branch'
    sh 'chmod a+x ./script.sh'
    sh './script.sh'
 }

 post { 
     always { 
	echo 'I will always say Hello again!'
	}
  }
}
