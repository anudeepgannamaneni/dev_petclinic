pipleline {
    agent { lable 'maven' }
       
       stages{
           stage('scm'){
               steps{
                   git branch: 'main', url: 'https://github.com/anudeepgannamaneni/dev_petclinic.git'
               }
           }
       }

}