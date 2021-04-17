node ('maven') {

   stage('SCM') {
      // git clone
	  git branch: 'main', url: 'https://github.com/anudeepgannamaneni/dev_petclinic.git'
   }
   stage('BUILD '){
      //build using maven
      sh 'mvn clean install'
   }
   stage('repots'){
      //all reopts 
      junit 'target/surefire-reports/*.xml'
   }
    stage('SonarQube analysis') {
    withSonarQubeEnv('sonarqube-6.7') { // You can override the credential to be used
      sh 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.7.0.1746:sonar'
    }
  }


}