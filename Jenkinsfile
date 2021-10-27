pipeline {
	agent any
	//agent { docker { image 'python:3.7.2' } }
	triggers { cron('H H(0-3) * * *') }
	
	
 	stages {
 		stage("Compile") {
 			steps {
 				echo "no need to build python code"
 			}
 		}
 		stage("Unit test") {
 			steps {
 				sh "python3 volume_cuboid_test.py"
 			}
 		}
 	}
}
