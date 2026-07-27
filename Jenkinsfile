pipeline{
	agent any

	stages{
		stage('Checkout'){
			steps{
				echo 'Repo already checked out by jenkins at this point'
				sh 'ls -la'
			}
		}

		stage('Build'){
			steps{
				echo 'Pretending to build something...'
			}
		}

		stage('Test'){
			steps{
				echo 'Pretending to test something...'
			}
		}
	}
}
