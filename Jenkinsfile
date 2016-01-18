#!groovy

stage 'Dev'
node ('master') {
	sh 'java --version'
	checkout scm
	sh "mvn clean install"
}