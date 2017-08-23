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
		echo 'I am in the build stage'
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
