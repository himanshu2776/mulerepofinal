pipeline
{

tools { 
      'Maven-3.6.3'
    }

stages {

stage("Build Application"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps {
bat 'mvn clean install'
}
}

stage("Deploy Application to mulesoft cloudhub"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps {
 bat 'mvn clean package deploy -Danypoint.username=hexa -Danypoint.password=Printout452009 -Danypoint.environment=Sandbox'
}
}
}
}

