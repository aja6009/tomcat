node{
   stage('SCM CHECKOUT'){
     git 'https://github.com/aja6009/tomcat'
}
   stage('Compile-package'){
      def mvnHome = tool name: 'MAVEN_HOME', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
}
   stage('email notification'){
      mail bcc: '', body: 'the project deployment has been completed the 99% call the manager to axis the report and send the result', cc: '', from: '', replyTo: '', subject: 'project report', to: 'ajayguru9562@gmail.com'
}
}
