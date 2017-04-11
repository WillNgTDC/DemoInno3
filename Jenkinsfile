pipeline {	
	agent any
	stages {
	stage('Stage1') {
	steps {
	parallel(
	"Stage1": {
	echo 'Stage1 Message'
	},
	"Stage1B": {
	echo 'Stage1B Message'
	}
	)
	}
	}
	stage('Stage2') {
	steps {
	parallel(
	"Stage2": {
	echo 'Stage2 Message'
	},
	"Stage2B": {
	echo 'Stage 2B Message'
	}
	)
	}
	}
	stage('Stage3') {
	steps {
	echo 'Stage3 Message'
	}
	}
	}
	}
