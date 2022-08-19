pipeline{

agent any

tools{
maven 'maven3.8.2'

}

stages{

  stage('CheckOutCode'){
    steps{
       scminfo = checkout scm
	
    }
  }
  
  stage('Build'){
  steps{
  sh  "mvn clean package"
  }
  }

  }
}
