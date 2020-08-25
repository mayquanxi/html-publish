pipeline {
	agent any
	stages {
		stage('publish html') {
			steps {
				publishHTML(
					allowMissing: false,
					reportName: 'Publish example',
					reportDir: '.',
					reportFiles: 'index.html',
					keepAll: true,
					//reportTitles: 'Publish title',
					alwaysLinkToLastBuild: true
				)
			}
		}
	}
}
//https://www.jenkins.io/doc/pipeline/steps/htmlpublisher/