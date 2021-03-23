node{
stage('scm checkout'){
git 'https://github.com/kumar-devopstraining/maven-project.git'
}
stage('package'){
define mvnhome = tool name: 'maven', type: 'maven'
sh "${mvnhome}/bin/mvn package"
}
}
