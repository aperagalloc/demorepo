#!/usr/bin/env groovy

pipeline {
	agent none
	stages {
		node {
			deleteDir()
			env.SOMEATTR = "SOME_ATTRIBUTE"
			env.OTHERATTR = "OTHER_ATTRIBUTE"

			someBuildStages()
		}
	}
}

def someBuildStages(){
  stage("\u27A1 Build Stage/UT"){
    ansiMessage("Build Stage Start/UT")
    sh "echo Hello World!"

    ansiMessage("\u2713 Build Stage Done/UT")
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