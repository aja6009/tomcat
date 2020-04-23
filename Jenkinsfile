node{
   stage('SCM CHECKOUT'){
     git 'https://github.com/aja6009/tomcat'
}
   stage('Compile-package'){
      def mvnHome = tool name: 'MAVEN_HOME', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
}
}
