pipeline
{

agent any


stages {

stage("Build Application"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }

}

stage("Deploy Application to mulesoft cloudhub"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }


}
}
}

