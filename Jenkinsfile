//def ReleaseDir = "c:\inetpub\wwwroot"
pipeline {
			agent any
			stages {
				stage('Source'){
					steps{
						checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'bac8d490-e142-4a5e-9629-34ecbd0c26dc', url: 'https://github.com/ABDSonata/Online-Examination-System/']]])
					}
				}
				
			        stage('Build') {
    				        steps {
    					    bat '"call C:\Program Files\Jenkins\checkone.bat /;"'
    					    
    					}
				}
			}	
}
