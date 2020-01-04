node {
stage('SCM Checkout'){    
    git 'https://github.com/ADiprashan/my-app'
}
stage('Complie Package') {
   def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
}
    
    stage ('Email Notification')    {
    
    mail bcc: '', body: 'Jenkintest', cc: '', from: '', replyTo: '', subject: 'Jenkintest', to: 'devdehi813@gmail.com'
    }

}
