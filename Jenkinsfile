pipeline{
	    
    tools{
        jdk 'myjava'
        maven 'mvnn'
    }

    agent { label 'kslave1' }
        
        stages{
            
            stage('Checkout'){
	    
                steps{
		            echo 'cloning..'
                    git 'https://github.com/lam-phanminh/ansible-end-project-1.git'
                    sh 'pwd'
                    sh 'whoami'
                }
            
            }

            stage('Install tools by ansible'){
	    
                steps{
                    
                    // ansiblePlaybook disableHostKeyChecking: true, installation: 'ansible-kslave1', inventory: 'inventory', playbook: 'playbook.yml'
                    sh 'pwd'
                }
            
            }
        }
}
