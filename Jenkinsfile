node{
stage('scm checkout'){
git branch: 'main', url: 'https://github.com/kumar-devopstraining/maven-project.git' 
}
stage('package'){
def mvnhome = tool name: 'maven', type: 'maven'
sh "${mvnhome}/bin/mvn package"
}
  Stage('shell command'){
  sh 'echo $BUILD_ID'
  }
}
