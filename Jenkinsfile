pipeline{
    agent{
        label 'main'
    }
    tools{
        maven 'maven'
        jdk 'jdk_11'
    }
    stages{
        stage(Check out the Code){
          step{
              git url : 'git@github.com:Yash-9/Bookzy.git' 
          }
        }
        stage(Compile Code){
            step{
               sh "mvn compile"
            }
        }
        stage(Junit test){
            step{
                sh "mvn test"
            }
        }
        
    }


}