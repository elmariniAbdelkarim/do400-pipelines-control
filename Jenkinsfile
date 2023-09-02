pipeline {
   agent { node { label  'nodejs' }}
   stages {	
     stage('run tests'){
      parallel {
   	stage('backend tests') { 
	  steps {
		sh 'node ./backend/test.js'
}}
        stage('frontend tests') {
	  steps {
		sh 'node ./frontend/test.js'}
}}}}}
