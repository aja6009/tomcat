node{
   stage('SCM CHECKOUT'){
     git 'https://github.com/aja6009/tomcat'
}
   stage('Compile-package'){
      def mvnHome = tool name: 'MAVEN_HOME', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
}
   stage('stack notifcation'){
     slackSend baseUrl: 'https://hooks.slack.com/services/', 
        channel: 'ajayrock', color: 'good', message: 
        'i can see the deploy in good conduction no issue are present', tokenCredentialId: 
        'the jenkins work', username: 'ajaygurugubilli9@gmail.com'
}
}
}
