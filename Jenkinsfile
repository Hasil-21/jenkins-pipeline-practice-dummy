pipeline{
	agent { label 'linux-agent' }

	stages{
		stage('Checkout'){
			steps{
				echo 'Repo already checked out by jenkins at this point'
				sh 'ls -la'
			}
		}

		stage('Where am i'){
			steps{
				sh 'hostname'
				sh 'whoami'
				sh 'pwd'
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

		stage('User secret'){
			steps{
				withCredentials([string(credentialsId:'demo-secret', variable:'MY_SECRET')]){
					sh 'echo "using secret now..."'
					sh 'echo $MY_SECRET'
				}
			}
		}
	}
}
