pipeline{
	
    agent { label 'kslave1' }
        
        stages{
            
            stage('Checkout'){
	    
                steps{
		            echo 'cloning..'
                    git 'https://github.com/lam-phanminh/ansible-end-project-1.git'
                }
            
            }

            stage('Install tools by ansible'){
	    
                steps{
                    ansiblePlaybook credentialsId: 'root-ansible', installation: 'ansible-kslave1', inventory: 'inventory', playbook: 'playbook.yml'
                }
            
            }
        }
}
