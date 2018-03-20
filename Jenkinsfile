#!/usr/bin/env groovy

pipeline {
	agent none
	stages {
		stage("\u27A1 Build Stage/UT") {
			steps {
				ansiColor("xterm") {
		    	sh "echo Hello World!"
	  		}
	  	}
		}

	  stage("Next Stage - 2") {
	  	steps {
	  		sh "echo Hello World! 2"
	  	}
	  }
	  
	  stage("Next Stage - 3") {
	  	steps {
	  		sh "echo Hello World! 3"
	  	}
	  }

	  stage("Next Stage - 4") {
	  	steps {
	  		sh "echo Hello World! 4"
	  	}
	  }
	}
}