pipeline
{

agent any

stages{

stage{'Build Application'}{
steps{
bat 'mvn clean install'
}
}

stage{'Deploy Application to mulesoft cloudhub'}{
steps{
bat 'package deploy -DmuleDeploy -Dusername=hexa -Dpassword=Printout452009 -Denvironment=Sandbox -Dmule.version=4.3.0'
}
}
}

}