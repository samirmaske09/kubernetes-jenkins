pipeline {
     agent any
     stages {
         
         stage('Pull') {
              steps {
                 echo "Build stage is running"
                 git branch: 'main', url: 'https://github.com/samirmaske09/kubernetes-jenkins.git'
                    }
                        }
         
         
         stage("Docker build"){
              steps {
                sshagent(['centos']) {
                    sh 'docker build -t .'
 
                               }

                     }
                              }      
                             
         
         stage('Test') {
              steps {
                 echo "Build stage is running"
                    }
                        }
         
         
         stage('Deploy') {
              steps {
                 echo "Build stage is running"
                    }
                         }
            }

}