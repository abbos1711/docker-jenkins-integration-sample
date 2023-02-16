node{
  stage('SCM CHeckout'){
    git 'https://github.com/abbos1711/docker-jenkins-integration-sample'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'Maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email Notification'){
    mail bcc: '', body: '''HI welcome to JEnkins mail
    It is interesting
    Be healthy''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'rewilderkevin@gmail.com'
  }
}
