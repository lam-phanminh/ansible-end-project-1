pipeline{
    tools{
        jdk 'myjava'
        maven 'mvnn'
    }
	//agent {label 'linux_slave'}
	agent any
      stages{
           stage('Checkout'){
	    
               steps{
		 echo 'cloning..'
                 git 'https://github.com/devops-learner01012022/DevOpsClassCodes.git'
              }
          }
        //   stage('Compile'){
             
        //       steps{
        //           echo 'compiling..'
        //           sh 'mvn compile'
	    //   }
        //   }
        //   stage('CodeReview'){
		  
        //       steps{
		    
		//   echo 'codeReview'
        //          // sh 'mvn pmd:pmd'
        //       }
        //   }
        //    stage('UnitTest'){
		  
        //       steps{
	         
        //           sh 'mvn test'
        //       }
        //        post {
        //        success {
        //            junit 'target/surefire-reports/*.xml'
        //        }
        //    }	
        //   }
//            stage('MetricCheck'){
              
//               steps{
//                   sh 'mvn cobertura:cobertura -Dcobertura.report.format=xml'
//               }
//                post {
//                success {
// 	           cobertura autoUpdateHealth: false, autoUpdateStability: false, coberturaReportFile: 'target/site/cobertura/coverage.xml', conditionalCoverageTargets: '70, 0, 0', failUnhealthy: false, failUnstable: false, lineCoverageTargets: '80, 0, 0', maxNumberOfBuilds: 0, methodCoverageTargets: '80, 0, 0', onlyStable: false, sourceEncoding: 'ASCII', zoomCoverageChart: false                  
//                }
//            }		
//           }
        //   stage('Package'){
		  
        //       steps{
		  
        //           sh 'mvn package'
        //       }
        //   }
	      
        //   stage('Build Image'){
		  
        //       steps{
		  
        //           sh 'docker build -t phanminhlam/myimage:$BUILD_NUMBER .'
        //       }
        //   } 
        //   stage('Push image to docker registry'){
		  
        //       steps{
		  
        //           sh 'docker login -u phanminhlam -p Phanminhlam1@'
		//           sh 'docker push phanminhlam/myimage:$BUILD_NUMBER'
        //       }
        //   }
	64 bytes from 8.8.8.8: icmp_seq=108 ttl=58 time=4359 ms
64 bytes from 8.8.8.8: icmp_seq=109 ttl=58 time=3362 ms
64 bytes from 8.8.8.8: icmp_seq=110 ttl=58 time=2334 ms
64 bytes from 8.8.8.8: icmp_seq=111 ttl=58 time=1314 ms
64 bytes from 8.8.8.8: icmp_seq=112 ttl=58 time=492 ms

                    //   publishers: [
                    //     sshPublisherDesc(
                    //       configName: 'slave1', 
                    //       sshCredentials: [
                    //         keyPath: '/var/lib/jenkins/slave-privatekey', 
                    //         username: 'root'
                    //         ], 
                    //       transfers: [
                    //         sshTransfer(
                    //           execCommand: 'docker login -u phanminhlam -p Phanminhlam1@ && docker pull phanminhlam/myimage:$BUILD_NUMBER && docker run -d phanminhlam/myimage:$BUILD_NUMBER'
                    //             // execCommand: 'echo "abcccccccccc"'
                    //           )
                    //         ]
                    //     )
                    //   ]
                    // )
                    // sh "ssh -i $SETCRET root@172.31.31.158 \"docker login -u phanminhlam -p Phanminhlam1@\""
                    // sh "ssh -i $SETCRET root@172.31.31.158 \"docker pull phanminhlam/myimage:$BUILD_NUMBER\""
                    sh "ssh -i $abczyx root@172.31.31.158 \"docker run -d phanminhlam/myimage:10\""
                }
            }
        }
      }
}
