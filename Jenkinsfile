pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				echo "Build ToyStore Project"
			}			
		}
		stage('Test'){
	           steps{
	               echo "Test ToyStore Project"
	           }
	       }
		   stage('Integration Test'){
	           steps{
	               echo "Integration Test ToyStore Project"
	           }
	       }
		

	}
		post{
	     always{
	            echo "Always running"
	            }
	     success{
		echo "Build successful"
		}
               failure{
		echo  "Build failure"
		}
	    changed{
		echo "change is triggered when a failed build become successful or a successful build fails"
		}
		
}
	
}



















// node{
// 	echo 'Build ToyStore '
// 	echo 'Test ToyStore Project'
// 	echo 'Int-Test ToyStore Project'
// }
// node {
// 	stage('Build') {
// 		echo "Build ToyStore Project"
// 	}
// 	stage('Test') {
// 		echo "Test ToyStore Project"
// 	}
// 	stage('Integeration Test') {
// 		echo "Int-Test ToyStore Project"
// 	}
// }

