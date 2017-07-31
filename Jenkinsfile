pipeline {
	agent any 

	stages {
		stage('build') {
			steps{
			sh '/bin/ant -f build.xml -v'
			
			}
		}
        }
	post {
		always{
			archive 'dist/*.jar'
		}

	}
}
