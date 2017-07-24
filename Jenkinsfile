pipeline
{
	agent any
	stages {
	{
	stage ('git code') {
	 properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('* * * * *')])])
	 checkout scm
	 }

	 stage('Build env') {
		sh 'sudo I am an error'
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
