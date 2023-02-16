node{
  stage('SCM CHeckout'){
    git 'https://github.com/abbos1711/docker-jenkins-integration-sample'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: '', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }


}
