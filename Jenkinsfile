pipeline {
   agent anynode
   stage('SCM Checkout'){
    git 'https://github.com/pavan3004/jenkins-example'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
