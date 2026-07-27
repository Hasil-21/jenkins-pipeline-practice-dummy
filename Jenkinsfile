@Library('my-shared-lib') _
pipeline{
	agent { label 'linux-agent' }

	stages{
		stage('Greet'){
			steps{
				greet('Hasil')
			}
		}
	}
}
