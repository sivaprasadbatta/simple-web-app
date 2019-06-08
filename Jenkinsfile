node{
  stage('SCM checkout'){
    git 'https://github.com/sivaprasadbatta/simple-web-app.git'
  }
  stage('compile-package'){
    def mavenhome=tool name: 'Maven', type: 'maven' //defing maven home path if jenkins is unable to find maven home path this we use this line,goto jenkins PIPELINE SYNTAX->select TOOL->select maven->Generate syntax=the out put is maven home directory , assign this to a variable(or) if jenkins automatically finding the maven path no need this step direcltlu use -->sh 'mvn package'
    
    sh "${mavenhome}/bin/mvn package"
  }
}
