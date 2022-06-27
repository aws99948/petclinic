pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
		        sh 'whoami'
                        sh 'helm upgrade --install petclinic-app petclinic  --set image.repository=registry.hub.docker.com/aws978707/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
