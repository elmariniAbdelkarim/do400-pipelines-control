pipeline {
   agent { node { label  'nodejs' }}
   parameters{
	booleanParam(name: "RUN_FRONTEND_TESTS", defaultValue: true)
}
   stages {	
     stage('run tests'){
      parallel {
   	stage('backend tests') { 
	  steps {
		sh 'node ./backend/test.js'
}}
        stage('frontend tests') {
	   when { expression {params.RUN_FRONTEND_TESTS }}	
	   steps {
			sh 'node ./frontend/test.js'}
}}}}}
