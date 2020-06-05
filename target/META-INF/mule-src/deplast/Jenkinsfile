pipeline
{

agent any


stages{

stage{"Build Application"}

{
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps{
 "mvn clean install"
}
}

stage{"Deploy Application to mulesoft cloudhub"}{
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps{
 "mvn package deploy -DmuleDeploy -Dusername=hexa -Dpassword=Printout452009 -Denvironment=Sandbox -Dmule.version=4.3.0"
}

}
}
}

