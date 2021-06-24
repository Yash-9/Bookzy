pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage("Checkout the Code"){
          steps{
              git url : 'git@github.com:Yash-9/Bookzy.git' 
          }
        }
        stage("Compile Code"){
            steps{
               sh "mvn compile"
            }
        }
        stage("Junit test"){
            steps{
                sh "mvn test"
            }
        }
        
    }


}
