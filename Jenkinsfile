#!/usr/bin/env groovy

env.SOMEATTR = "SOME_ATTRIBUTE"
env.OTHERATTR = "OTHER_ATTRIBUTE"

node { 
		if (env.BRANCH_NAME == 'master') {

			stage("\u27A1 Build Stage") {
	    	sh "echo Hello World!"
			}

		  stage("Next Stage - 2") {
		  		sh "echo Hello World! 2"
		  		if (env.SOMEATTR.contains("SOME_ATTRIBUTE")) {
		  			sh "echo SOME_ATTRIBUTE"
		  		}


		  		if (env.OTHERATTR.contains("OTHER_ATTRIBUTE")) {
		  			sh "echo $env.OTHERATTR"
		  		}
		  }
		  
			  	stage("Next Stage - 3") {
				  	ansiColor("xterm") {
				  		sh "echo Hello World! 3"
				  		echo "http://www.something.com"
				  	}
			  		echo "http://www.something.com"
			  	}
			 
				  stage("Next Stage - 4") {
			  		sh "echo Hello World! 4"
			  		withEnv(['env1=ambiente1']) {
			  			sh "sleep 3"
			  			sh "echo $env1"
			  		}
				  }
		  

		  stage("Next Stage - 5") {
		  		sh "echo Hello World! 5"
		  		if (isUnix()) {
		  			sh "echo unix"
		  		}
		  }
		}

		if (env.BRANCH_NAME == 'otherbranch') {
		  someBuildStage("'otro branch $env.BRANCH_NAME'")
		}
}


def someBuildStage(message) {
	stage("OTHERBRANCH stage 1") {
		sh "echo $message"
	}
}