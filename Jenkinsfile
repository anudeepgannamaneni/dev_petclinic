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
      junit 'target/surefire-repots/*.xml'
   }


}