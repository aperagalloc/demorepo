#!/usr/bin/env groovy

node {
		stage("\u27A1 Build Stage") {
			env.SOMEATTR = "SOME_ATTRIBUTE"
			env.OTHERATTR = "OTHER_ATTRIBUTE"
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
	  			sh "echo $env1"
	  		}
	  }
}