node{
  stage('SCM checkout'){
    git 'https://github.com/sivaprasadbatta/simple-web-app.git'
  }
  stage('compile-package'){
    sh 'mvn package'
  }
}
