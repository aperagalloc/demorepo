#!/usr/bin/env groovy

node {
		stage("\u27A1 Build Stage") {
			env.SOMEATTR = "SOME_ATTRIBUTE"
			env.OTHERATTR = "OTHER_ATTRIBUTE"
		    	sh "echo Hello World!"
		    	sh "echo ${env.SOMEATTR}
		}

	  stage("Next Stage - 2") {
	  		sh "echo Hello World! 2"
	  }
	  
	  stage("Next Stage - 3") {
	  		sh "echo Hello World! 3"
	  }

	  stage("Next Stage - 4") {
	  		sh "echo Hello World! 4"
	  }
}