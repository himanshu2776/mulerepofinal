pipeline
{

agent any


stages {

stage("Build Application"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps {
echo 'This is a minimal pipeline.'
}
}

stage("Deploy Application to mulesoft cloudhub"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps {
 echo 'This is a other pipeline.'
}

}
}
}

