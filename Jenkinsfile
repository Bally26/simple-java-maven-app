pipeline{
	agent{
		docker{
			image 'maven'
			args '-v /root/.m2:/root/.m2'
		}
	}
	stages{
			stage('build'){
				steps{
					sh 'mvn -b -DskipTests clean package'
					}
			}
	}	
	
}