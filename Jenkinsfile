#!groovy

stage 'Dev'
node ('master') {
	sh 'java -version'
	checkout scm
	sh "/usr/local/apache-maven/apache-maven-3.3.9/bin/mvn clean install"
}