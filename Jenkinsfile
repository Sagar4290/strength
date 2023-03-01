node{
  stage('scm checkout'){
    git 'https://github.com/Sagar4290/strength.git'
  }
  stage('compile-package'){
    def mvnHome=tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email Notification'){
    mail bcc: '', body: 'Hello jenkins', cc: '', from: '', replyTo: '', subject: 'Jenkinsjob', to: 'sagarkul13@gmail.com'
  }
}
