node{
stage('scm checkout'){
checkout changelog: false, scm: [$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/kumar-devopstraining/maven-project.git']]]
}
stage('package'){
define mvnhome = tool name: 'maven', type: 'maven'
sh "${mvnhome}/bin/mvn package"
}
}
