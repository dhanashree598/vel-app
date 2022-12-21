pipeline {

		agent {
                         label {
                                    label 'built-in'
                                    customWorkspace '/mnt/myproject'
                         }
                }
		
		stages {
		
			stage ('deploy') {
			
				steps {
				
				    sh "cp -r index.html /var/www/html"
					sh "chmod -R 777 /var/www/html/index.html"
				
				}
			
			}
			
			stage ('restart') {
			
				steps {
				
				    sh "service htttpd restart"
				
				}
			
			}
                }
}
			
