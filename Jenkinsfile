#!groovy

stage 'Dev'
node ('master') {
	sh 'java -version'
	checkout scm
	sh "mvn clean install"
}
stage 'Release'
node ('master') {
 	sh 'ls /root/repository/'
	sh 'whoami'
	sh 'cp /var/lib/jenkins/.m2/repository/com/walmart/weekly-dashboard-automation/0.0.2-SNAPSHOT/weekly-dashboard-automation-0.0.2-SNAPSHOT.war /root/repository/'
	
		}
