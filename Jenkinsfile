node('nodejs') {
   stage('checkout') {
	git branch: 'main', url: 'https://github.com/elmariniAbdelkarim/do400-pipelines-control.git'
}
   stage('backend tests') { 
	sh 'node ./backend/test.js'
}
   stage('frontend tests') {

	sh 'node ./frontend/test.js'}
}
