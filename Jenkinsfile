stage('Sonar Scan'){
		sonar{
			buildType = 'MAVEN'
			runScan = true
			pomFileLocation = 'sonar-scanner-jenkins/pom.xml'
			analysisParameters = "mvn sonar:sonar -Dsonar.exclusions=*.java"
		}
	}
}
