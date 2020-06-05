pipeline
{

agent any
 triggers { cron('* * * * *') }

stages {

stage("Build Application"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps {
echo 'mvn clean install'
}
}

stage("Deploy Application to mulesoft cloudhub"){
environment {
        ANYPOINT_CREDENTIALS = credentials("anypoint.credentials") 
      }
steps {
 echo 'mvn clean package deploy -Danypoint.username=hexa -Danypoint.password=Printout452009 -Danypoint.environment=Sandbox'
}

}
}
}

