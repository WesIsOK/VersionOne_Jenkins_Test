pipeline
{
	agent any
	stages {
	stage ('git code') 
	{
		steps {
		checkout scm
		}
	}

	 stage('Build env') 
	 {
	 steps {
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
