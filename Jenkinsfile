#!/usr/bin/env groovy

pipeline {
	agent none
	stages {
		stage("\u27A1 Build Stage/UT") {
			steps {
				ansiMessage("Build Stage Start/UT")
		    sh "echo Hello World!"
	    	ansiMessage("\u2713 Build Stage Done/UT")
	  	}
		}

	  stage("Next Stage - 2") {
	  	steps {
	  		sh "echo Hello World! 2"
	  	}
	  }
	  
	  stage("Next Stage - 3") {
	  	steps {
	  		sh "echo Hello World! 2"
	  	}
	  }

	  stage("Next Stage - 4") {
	  	steps {
	  		sh "echo Hello World! 2"
	  	}
	  }
	}
}