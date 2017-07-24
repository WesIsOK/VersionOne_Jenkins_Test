https://www14.v1host.com/LaureateSandbox
https://community.versionone.com/VersionOne_Connect/Supported_Integrations/VersionOne_Integration_for_Jenkins
http://v1appcatalog.azurewebsites.net/app/index.html#/Details/VersionOne.Integration.Jenkins


#!groovy

import groovy.json.JsonOutput
import groovy.io.FileType

pipeline
{
	agent any
	stages {
	{
	stage ('git code') 
	{
		steps {
		properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('* * * * *')])])
		checkout scm
		}
	}

	 stage('Build env') 
	 {
	 steps {
		sh 'sudo I am an error'
		sh 'echo I am not the master branch'
		sh 'chmod a+x ./script.sh'
		sh './script.sh'
		}
	 }
	}
	post
	{ 
		always { 
			echo 'I will always say Hello again!'
		}
	}

}
