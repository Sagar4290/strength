node{
  stage('scm checkout'){
    git 'https://github.com/Sagar4290/strength.git'
  }
  stage('compile-package'){
    def mvnHome=tool name: 'maven-3', type: 'maven'
    sh "${mvnHome} /bin/mvn package"
  }
}
