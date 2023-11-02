@Library('jenkins_shared_lib') _

pipeline{

    agent any

     stages{
        
        stage('Git Checkout'){
               when { expression {  params.action == 'create' } }
            steps{
            gitCheckout(
                branch: "main",
                url: "https://github.com/manikanta225/Bamboo.git"
            )
            }
        }
             stage('Unit Test maven'){
         
         when { expression {  params.action == 'create' } }

            steps{
               script{
                   
                   mvnTest()
               }
            }
        }
     
     
     
     
     
     
     
     
     }





    






    
}
