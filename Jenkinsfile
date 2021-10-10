node{
     tools{
     maven 'maven363'
  }
      stage("Checkout"){
	   git 'git@github.com:Sathish-QA/myProjectJava.git'
	   }
	stage("Build"){
	   sh 'mvn clean compile'
	   }
	stage("Test"){
	   sh 'mvn test'
	   junit '**/target/surefire-reports/TEST-*.xml'
	  }
	stage("Package") {
	     sh "mvn package"
	}
	   
}
