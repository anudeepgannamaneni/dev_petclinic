pipeline{
    agent{
        node{
            lable 'maven'
        }
    }
    stages {
        stage('scm'){
            steps{
                //To clone git repositary
                git branch: 'main', url: 'https://github.com/anudeepgannamaneni/dev_petclinic.git'
                

            }
        }
    }




}


